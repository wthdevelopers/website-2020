<template>
  <div>
    <SubHeader>{{ title }}</SubHeader>
    <Accordion
      v-for="data in accordionData"
      :key="data.id"
      :accordionId="data.id"
      :open="data.id === defaultOpenId"
      :accordionName="accordionGroupId"
      :onClick="onTrigger"
    >
      <template v-slot:title>{{ data.title }}</template>
      <Para v-if="data.type === 'text'" style="margin: 30px 0 20px 0;">{{ data.content }}</Para>
      <Location v-if="data.type === 'location'" />
    </Accordion>
  </div>
</template>
<script>
import SubHeader from '@/components/SubHeader';
import Accordion from '@/components/Accordion';
import Para from '@/components/Para';
import Location from '@/components/Location';

export default {
  components: { Accordion, SubHeader, Para, Location },
  data: function() {
    return {
      accordionData: this.content,
      accordionGroupId: this.title
        .toLowerCase()
        .split(' ')
        .join('-'),
    };
  },
  props: {
    title: {
      type: String,
      required: true,
    },
    content: {
      type: Array,
      required: true,
    },
    defaultOpenId: {
      type: Number,
    },
    onClick: {
      type: Function,
      required: true,
    },
  },
  methods: {
    onTrigger(id) {
      this.onClick(id);
    },
  },
};
</script>

<style lang="css" scoped>
h4 {
  margin-top: 100px;
}
</style>
