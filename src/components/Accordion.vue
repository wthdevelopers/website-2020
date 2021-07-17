<template>
  <div :class="['accordion', { 'accordion-open': highlighted }]" :id="`${accordionName}-${accordionId}`">
    <h4>
      <button
        type="button"
        class="accordion-trigger"
        :id="`${accordionName}-trigger-${accordionId}`"
        :aria-expanded="expanded ? 'true' : 'false'"
        :aria-controls="`${accordionName}-content-${accordionId}`"
        @click="onClickHandler"
      >
        <span class="accordion-title" :id="`${accordionName}-title-${accordionId}`">
          <slot name="title"></slot>
        </span>
        <svg
          class="accordion-arrow"
          :id="`${accordionName}-arrow-${accordionId}`"
          viewBox="0 0 50.07 28.56"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="m25 28.52a3.48 3.48 0 0 1 -2.48-1l-21.52-21.52a3.54 3.54 0 0 1 5-5l19 19 19-19a3.54 3.54 0 0 1 5 5l-21.53 21.49a3.48 3.48 0 0 1 -2.48 1z"
            transform="translate(.04 .04)"
          ></path>
        </svg>
      </button>
    </h4>
    <div style="overflow: hidden">
      <div
        :class="['accordion-content', { 'accordion-content-open': expanded }]"
        :id="`${accordionName}-content-${accordionId}`"
        role="region"
        :aria-labelledby="`${accordionName}-trigger-${accordionId}`"
      >
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'accordion',
  data() {
    return {
      highlighted: this.open,
      expanded: this.open,
    };
  },
  props: {
    accordionId: {
      type: [String, Number],
      required: true,
    },
    accordionName: {
      type: String,
      required: true,
    },
    open: {
      type: Boolean,
      default: undefined,
    },
    onClick: {
      type: Function,
    },
  },
  watch: {
    open: function() {
      this.toggleAccordion();
    },
  },
  methods: {
    onClickHandler() {
      this.toggleAccordion();
      if (this.onClick) {
        this.onClick(this.accordionId);
      }
    },
    toggleAccordion() {
      if (this.open === undefined) {
        this.expanded = !this.expanded;

        if (this.highlighted) {
          setTimeout(() => {
            this.highlighted = false;
          }, 500);
        } else {
          this.highlighted = true;
        }
      } else {
        this.expanded = this.open;

        if (this.highlighted && !this.open) {
          setTimeout(() => {
            this.highlighted = false;
          }, 500);
        } else if (!this.highlighted && this.open) {
          this.highlighted = this.open;
        }
      }
    },
  },
};
</script>

<style scoped>
.accordion:first-of-type {
  margin-top: 50px;
}

.accordion {
  border: 2px solid var(--color-regular-text);
}

.accordion.accordion-open {
  border-color: var(--color-accent);
}

.accordion.accordion-open .accordion-title {
  color: var(--color-accent);
}

.accordion.accordion-open .accordion-arrow * {
  fill: var(--color-accent);
}

.accordion + .accordion {
  margin-top: 50px;
}

.accordion-trigger {
  display: flex;
  align-items: center;
  text-align: left;
  padding: 20px 30px;
  width: 100%;
}

.accordion-title {
  font-family: var(--font-primary), sans-serif;
  font-size: 24px;
  font-weight: 400;
  color: var(--color-regular-text);
  margin-right: auto;
}

.accordion-cancel {
  width: 17.5px;
  height: 17.5px;
  transform: translateY(2.5px);
}

.accordion-arrow {
  margin-left: 30px;
  width: 25px;
  height: calc((17.5px / 1.753) + 5px);
}

svg > path {
  fill: var(--color-regular-text);
}

.accordion-content {
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.6s ease-out;

  padding: 0 30px;
}

.accordion-content-open {
  max-height: 100vh;
}

@media (--mobile-narrow) {
  .accordion-trigger {
    padding: 5px 15px;
  }

  .accordion-title {
    font-size: 20px;
  }

  .accordion-cancel {
    width: 13px;
    height: 13px;
    transform: translateY(4.5px);
  }

  .accordion-arrow {
    width: 20px;
    margin-left: 20px;
    height: calc((20px / 1.753) - 1px);
  }
  .accordion-content {
    padding: 5px 15px;
  }
}
</style>
