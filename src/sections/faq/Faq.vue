<template>
  <section id="faq" title="FAQs">
    <SectionHeader>FAQs</SectionHeader>
    <div class="faq-content">
      <AccordionGroup
        v-for="(item, idx) in faqArr"
        :key="idx"
        :title="item.title"
        :defaultOpenId="currentOpenId"
        :content="item.content"
        :onClick="accordionGroupOnClickHandler"
      />
    </div>
    <svg id="solarscape" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 3093.3 1268.9">
      <g class="base">
        <path
          fill="#79c89f"
          d="M0 1173l129-16c129-16 387-48 644-43 258 6 516 48 774 48 257 0 515-42 773-69s516-37 644-43l129-5v224H0z"
        ></path>
        <path
          fill="#79c89f"
          d="M2773 1074l-21-1c-13-4-19-12-22-24-6-23-2-44 4-66l2-5 11-17c16-21 44-22 62-2a42 42 0 019 13 22 22 0 003 3c5 19 10 38 8 58a86 86 0 010 9c-5 24-14 32-39 32h-7c-7-6-3-15-5-23-2 8 2 17-5 23z"
        ></path>
        <path
          fill="#818fdb"
          d="M2773 1074l1-27c0-3 0-7 4-6 3 0 4 3 4 6l1 27-1 37c0 3 0 7-5 6-3 0-3-4-3-6l-1-37z"
        ></path>
        <path fill="none" stroke="#1023c3" stroke-miterlimit="10" stroke-width="25" d="M1992 1111v62"></path>
        <path fill="#1023c3" d="M1966 1191l-238-19 85-153 249-17-96 189z"></path>
        <path fill="none" stroke="#c36" stroke-miterlimit="10" stroke-width="25" d="M2336 1075v69"></path>
        <path fill="#c36" d="M2307 1163l-263-21 94-168 275-20-106 209z"></path>
        <path
          fill="#fff"
          d="M151 1172c-4 15-5 16-15 17h-8c-4-10-1-21-2-30-2 9 2 20-4 29a72 72 0 01-8 0c-9 0-13-5-13-19a195 195 0 0115-76c7-13 13-13 20 0 7 16 10 34 13 53a170 170 0 012 26z"
        ></path>
        <path fill="#8490dd" d="M122 1188l1-35c0-2-1-6 2-6 3-1 3 3 3 6v69c0 5 0 9-3 12-3-5-2-10-2-15v-23l-1-8z"></path>
        <path
          fill="#b8e2cc"
          d="M2821 1099c-2-21 3-40 5-60 5-12 7-25 13-37a91 91 0 016-11c8-12 12-13 23-2 10 17 16 35 19 54l2 3c4 5 4 11 3 16v27c0 18-7 25-25 26h-6c-6-5-4-12-4-18l-1-32c-2 15 5 33-4 50h-6c-12 0-20-5-25-16z"
        ></path>
        <path
          fill="#828fdc"
          d="M2852 1114l1-40a87 87 0 010-9 4 4 0 013-3c3-1 4 1 4 3v15l1 35-1 40a52 52 0 010 9 3 3 0 01-4 2l-3-2a60 60 0 010-9l-1-40z"
        ></path>
        <path
          fill="#fff"
          d="M295 1113c-4 11-5 12-17 12h-9c-5-7-1-15-3-22-2 7 3 15-4 21l-9 1c-11-1-15-4-16-14 0-13 4-26 9-38 2-6 5-12 9-17 8-9 15-9 23 0 9 11 12 25 15 38a78 78 0 012 19z"
        ></path>
        <path fill="#8490dd" d="M262 1124l1-25c0-1-1-4 2-4 3-1 4 2 4 4v50c0 4 0 7-4 9-3-4-2-8-2-11v-17l-1-6z"></path>
        <path fill="#d65c85" d="M668 997h206v150H668z"></path>
        <path fill="#c36" d="M873 997H668l-63-96 211-1 57 97z"></path>
        <path fill="#ebadc2" d="M542 1147V997l63-96 63 96 1 151-127-1z"></path>
        <rect width="21.2" height="16.9" x="564.4" y="1042" fill="#d65c85" rx="3.2"></rect>
        <rect width="21.2" height="16.9" x="620.6" y="1071.9" fill="#d65c85" rx="3.2"></rect>
        <path
          fill="#b8e2cc"
          d="M140 1154c-1-15 2-29 4-44 3-8 5-18 9-26a65 65 0 015-8c5-9 8-9 16-2a116 116 0 0114 40l2 2c3 3 2 7 1 12l1 19c0 13-5 18-18 19h-5c-4-4-3-9-3-13v-23c-2 10 3 23-3 36h-5c-9 0-15-4-18-12z"
        ></path>
        <path
          fill="#828fdc"
          d="M163 1166v-30a62 62 0 010-6 3 3 0 012-3c2 0 3 1 3 3l1 10v55a38 38 0 01-1 6 2 2 0 01-2 2h-1l-2-2a43 43 0 010-6v-29z"
        ></path>
        <path
          fill="#79c89f"
          d="M1054 1121l-16-1c-9-3-14-11-16-22-4-19-2-38 3-57l1-5 9-15c12-18 33-19 46-2a38 38 0 016 12 18 18 0 003 2c4 17 7 34 6 52v8c-4 21-11 28-29 28h-6c-5-6-2-14-3-20-1 7 2 14-4 20z"
        ></path>
        <path fill="#818fdb" d="M1054 1121l1-24c0-2 0-6 3-5 2 0 3 2 3 5v56c0 3 0 7-4 6-2 0-2-4-2-6l-1-32z"></path>
        <path
          fill="#b8e2cc"
          d="M166 1106c-1-22 3-44 6-66 5-14 8-28 14-41a101 101 0 017-12c9-14 13-14 26-3 10 19 17 39 20 61l3 3c4 5 4 11 2 18l1 30c0 20-8 27-28 28h-7c-6-6-4-13-4-19l-1-36c-2 16 6 36-4 55h-7c-14 0-23-5-27-18z"
        ></path>
        <path
          fill="#828fdc"
          d="M201 1123v-44a92 92 0 011-10 4 4 0 013-4c3-1 4 2 4 4l1 16v83a57 57 0 01-1 10 3 3 0 01-4 3l-3-3a66 66 0 01-1-10v-44z"
        ></path>
        <path
          fill="#b8e2cc"
          d="M278 1113c-2-17 4-32 7-48 7-10 10-20 18-29a75 75 0 019-9c11-10 17-10 32-2 13 14 23 28 27 44l2 2c6 4 6 8 4 13v21c0 14-9 20-35 20h-9c-7-4-5-9-5-13-1-10 1-19-1-26-3 12 7 26-5 39h-9c-17 1-29-3-35-12z"
        ></path>
        <path
          fill="#828fdc"
          d="M322 1125v-32a39 39 0 011-7c0-1 1-3 4-3 4 0 5 1 6 3a99 99 0 010 11l1 28-1 32a24 24 0 01-1 7c0 2-2 2-5 2l-4-2a27 27 0 01-1-7v-32z"
        ></path>
        <path
          fill="#79c89f"
          d="M1011 1158l-10-1c-6-3-8-11-9-21-3-20-1-39 2-58v-5l5-15c7-18 19-19 27-2a51 51 0 014 12 18 18 0 001 2 271 271 0 014 60c-2 21-6 28-17 28h-3c-3-5-1-13-2-20-1 7 1 15-2 20z"
        ></path>
        <path fill="#818fdb" d="M1011 1158v-24l1-5c2 0 2 3 2 5l1 24-1 32c0 3 0 7-2 6l-1-6v-32z"></path>
        <path
          fill="#fff"
          d="M996 1104c-4 15-5 16-15 16l-7 1c-5-10-2-21-3-30-2 9 2 20-3 29a75 75 0 01-9 0c-9 0-13-5-13-19a195 195 0 0115-76c7-13 13-13 20 0 7 16 10 34 13 52a171 171 0 012 27z"
        ></path>
        <path fill="#8490dd" d="M968 1120v-35c0-2 0-6 2-6 3-1 3 3 3 6l1 36v33c0 5-1 9-4 12-2-5-2-10-2-15v-23-8z"></path>
        <path
          fill="#79c89f"
          d="M927 1140l-18-1c-11-3-16-10-18-20-5-19-2-37 3-55l2-5 9-14c14-17 37-18 52-2a35 35 0 017 11 18 18 0 003 3c5 16 9 32 7 49a73 73 0 010 7c-4 20-12 27-33 28h-6c-5-6-2-14-4-20-1 6 2 14-4 19z"
        ></path>
        <path fill="#818fdb" d="M927 1140l1-22c0-3 0-6 3-6s4 3 4 6v53c0 3 0 6-4 6-4-1-3-4-3-6l-1-31z"></path>
        <path
          fill="#79c89f"
          d="M453 1180l-14-1c-8-2-11-9-13-18-4-16-2-32 2-48l1-4 7-12c10-15 28-16 39-2a32 32 0 015 10 15 15 0 002 2 134 134 0 015 50c-3 17-9 23-24 23h-5c-4-5-1-11-3-17-1 6 2 12-3 17z"
        ></path>
        <path fill="#818fdb" d="M453 1180v-20c0-2 0-5 2-4 2 0 3 2 3 4v47c0 2 0 5-3 5-2-1-2-3-2-5v-27z"></path>
        <path
          fill="#fff"
          d="M521 1134c-4 15-5 16-15 17h-8c-4-10-1-21-2-30-2 9 2 20-4 29a77 77 0 01-8 1c-9-1-13-6-13-20a195 195 0 0115-76c7-13 13-13 20 0 7 16 10 34 13 53a172 172 0 012 26z"
        ></path>
        <path fill="#8490dd" d="M492 1150l1-35c0-2-1-6 2-6 3-1 3 3 3 6v70c0 4 0 9-3 11-2-5-2-10-2-15v-23l-1-8z"></path>
        <path
          fill="#fff"
          d="M344 1194c-5 10-6 11-18 12h-8c-6-7-2-15-3-22-2 7 3 15-4 21h-10c-11 0-15-4-16-14 0-13 4-25 9-37 2-6 5-12 9-17 8-10 16-10 23 0 9 11 12 24 15 38a78 78 0 013 19z"
        ></path>
        <path fill="#8490dd" d="M311 1205v-25c0-2 0-4 2-5 4 0 4 2 4 5l1 26v24c0 3 0 7-4 8-3-3-3-7-3-11v-16-6z"></path>
        <path
          fill="#b8e2cc"
          d="M334 1217c-1-10 1-20 3-30l6-18a45 45 0 013-6c4-6 6-6 12-1a80 80 0 019 27l1 2c2 2 2 5 1 8v13c0 9-3 13-12 13h-3c-3-3-2-6-2-9v-16c-1 8 2 16-2 25h-4c-6 0-10-2-12-8z"
        ></path>
        <path
          fill="#828fdc"
          d="M350 1225v-20a45 45 0 010-5 2 2 0 011-2c2 0 2 1 2 2l1 7v38a26 26 0 01-1 4 2 2 0 01-1 2h-1l-1-1a30 30 0 010-5v-20z"
        ></path>
        <path
          fill="#b8e2cc"
          d="M1252 1179c-1-11 2-22 3-33l7-20a49 49 0 013-6c5-7 7-7 13-1a87 87 0 0110 30l1 1c2 3 2 6 2 9v15c0 9-4 13-14 13h-3c-3-2-2-6-3-9v-18c-1 8 3 18-2 27h-3c-7 1-11-2-14-8z"
        ></path>
        <path
          fill="#828fdc"
          d="M1269 1187v-22a47 47 0 010-4 2 2 0 012-2c2-1 2 0 2 2l1 7v41a28 28 0 01-1 5 2 2 0 01-2 1l-1-1a33 33 0 01-1-5v-22z"
        ></path>
        <path
          fill="#b8e2cc"
          d="M843 1163c-1-15 2-29 4-43l9-26a65 65 0 014-7c6-9 9-9 17-2a113 113 0 0113 39l1 2c3 3 3 7 2 11v19c0 13-5 18-17 18h-5c-4-3-3-8-3-12v-23c-1 10 4 23-3 35h-4c-9 0-15-3-18-11z"
        ></path>
        <path
          fill="#828fdc"
          d="M865 1174v-29a59 59 0 011-6 3 3 0 012-2c2-1 3 1 3 2v63a37 37 0 010 7 2 2 0 01-3 1l-2-1a42 42 0 01-1-7v-28z"
        ></path>
        <path fill="none" stroke="#1023c3" stroke-miterlimit="10" stroke-width="25" d="M2709 1142v62"></path>
        <path fill="#1023c3" d="M2683 1222l-239-20 86-152 249-18-96 190z"></path>
      </g>
      <g id="solarscape-panels-one" fill="#d65c85">
        <path d="M2300 1154l-241-20 86-154 251-16-96 190zM864 991H673l-59-86 196-1 54 87z"></path>
      </g>
      <g id="solarscape-panels-two" fill="#404fcf">
        <path d="M1960 1183l-219-18 78-140 228-15-87 173zM2677 1213l-219-18 78-140 228-14-87 172z"></path>
      </g>
      <g id="solarscape-panel-dividers" fill="none" stroke-miterlimit="10">
        <path
          stroke="#1023c3"
          stroke-width="10"
          d="M1886 1018l-84 157M1974 1011l-91 171M1791 1066l234-5M1761 1120l233 5"
        ></path>
        <path
          stroke="#c36"
          stroke-width="10"
          d="M2218 972l-92 174M2315 965l-100 188M2114 1026l258-6M2081 1085l257 5"
        ></path>
        <path stroke="#c36" stroke-width="5" d="M627 930h203M648 962h203M740 993l-60-90M808 993l-61-90"></path>
        <path
          stroke="#1023c3"
          stroke-width="10"
          d="M2602 1048l-83 158M2690 1042l-91 170M2508 1097l233-6M2478 1150l233 5"
        ></path>
      </g>
      <g class="lights-pink" fill="#d65c85">
        <rect width="21.2" height="16.9" x="620.4" y="1042" rx="3.2"></rect>
        <rect width="21.2" height="16.9" x="564.4" y="1071.9" rx="3.2"></rect>
      </g>
      <path
        class="cloud"
        id="solarscape-cloud-one"
        fill="#fff"
        d="M358 939H177c-10 0-16-3-18-13l-3-16c-1-29 17-41 48-34l5 1c15 4 17 3 18-12 1-29 10-56 32-79 37-37 106-28 130 16 9 17 9 16 29 12a79 79 0 0132 0c20 5 27 20 31 36a59 59 0 011 10c1 14 4 23 21 27 19 4 26 18 28 35 1 13-4 18-18 18H358z"
        opacity=".8"
      ></path>
      <path
        class="cloud"
        id="solarscape-cloud-two"
        fill="#fff"
        d="M1102 1081H986c-9 0-8 1-8-7 1-6 4-8 10-9s6-2 7-7c1-6 1-12 4-18s9-11 18-12l12 2c6 1 6 1 6-4 0-11 6-20 13-28s17-14 29-16c13-2 25 1 35 8 11 8 17 18 22 30 2 5 2 5 8 2 8-4 17-4 25-3 17 3 27 12 32 25a23 23 0 012 6c0 2 1 3 4 3a51 51 0 019 2c9 2 13 7 13 13l1 10c0 2-1 3-3 3h-123z"
        opacity=".8"
      ></path>
      <path
        class="cloud"
        id="solarscape-cloud-three"
        fill="#fff"
        d="M2790 986l5 2c4 3 6 6 5 10l-3 3h-194c-5 0-8-1-10-5-8-14 0-28 18-31 8-1 8-1 8-8 1-7 2-14 8-19 9-8 20-8 31-4 2 1 5 2 6-1 4-13 16-18 28-23 14-6 39 1 49 16a83 83 0 016 12c2 3 4 4 9 3 7-2 14 1 17 6v4c-1 4 0 4 4 5 18 1 24 18 15 26l-2 4z"
        opacity=".8"
      ></path>
      <g class="stars-one" fill="#f9f458">
        <path
          d="M432 383a36 36 0 0011-6 20 20 0 006-9 58 58 0 002-9l2-7v2a113 113 0 004 15l1 2a11 11 0 003 4 52 52 0 008 6l4 2h1l-4 2a39 39 0 00-9 6 16 16 0 00-3 3 23 23 0 00-2 5 92 92 0 00-3 11v5h-1v-1a142 142 0 00-3-14l-2-6a13 13 0 00-4-5 36 36 0 00-8-5l-3-1h-1zM2788 628a36 36 0 0011-6 20 20 0 006-8 58 58 0 003-10l1-7v2a113 113 0 004 15l1 2a11 11 0 003 5 51 51 0 008 5l4 2h1l-3 2a40 40 0 00-10 6 17 17 0 00-3 3 24 24 0 00-2 6 93 93 0 00-3 11v4h-1a144 144 0 00-3-15l-2-5a13 13 0 00-4-5 36 36 0 00-8-5l-3-1v-1z"
        ></path>
      </g>
      <g class="stars-two" fill="#f9f458">
        <path
          d="M1607 366l1-1a36 36 0 0011-6 20 20 0 006-8 58 58 0 002-10l1-6v-1l1 2a114 114 0 004 15l1 3a11 11 0 003 4 53 53 0 008 5l4 2v1l-3 1a40 40 0 00-9 6 17 17 0 00-3 4 23 23 0 00-2 5 95 95 0 00-3 11l-1 4a140 140 0 00-3-15l-2-5a13 13 0 00-4-5 36 36 0 00-8-5l-3-1h-1zM2590 31a35 35 0 0011-6 20 20 0 006-9 56 56 0 003-9l1-7v2a116 116 0 004 15l1 2a11 11 0 004 5 53 53 0 008 5l4 2-3 2a40 40 0 00-9 6 16 16 0 00-4 3 24 24 0 00-2 5 96 96 0 00-2 11l-1 5v-1a137 137 0 00-4-14l-2-5a13 13 0 00-4-6 35 35 0 00-8-4l-3-2z"
        ></path>
      </g>
      <g class="stars-three" fill="#f9f458">
        <path
          d="M80 723v-1a36 36 0 0011-6 20 20 0 006-8 58 58 0 003-10l1-7v2a113 113 0 004 15l1 3a11 11 0 004 4 53 53 0 008 5l4 2v1l-3 1a39 39 0 00-9 6 16 16 0 00-4 4 23 23 0 00-2 5 92 92 0 00-2 11l-1 4a140 140 0 00-4-15l-2-5a13 13 0 00-4-5 36 36 0 00-8-5l-3-1zM1322 568a36 36 0 0011-6 20 20 0 006-9 58 58 0 003-9l1-7 1 2a113 113 0 003 15l2 2a11 11 0 003 5 52 52 0 008 5l4 2-3 2a39 39 0 00-9 6 16 16 0 00-3 3 23 23 0 00-2 5 92 92 0 00-3 11l-1 5v-1a143 143 0 00-4-14l-2-5a13 13 0 00-4-6 36 36 0 00-8-5l-3-1z"
        ></path>
      </g>
    </svg>
  </section>
</template>

<script>
import SectionHeader from '@/components/SectionHeader.vue';
import AccordionGroup from '@/components/AccordionGroup';
import { faqData } from '@/sections/faq/faqData';

export default {
  name: 'faq',
  components: {
    AccordionGroup,
    SectionHeader,
  },
  data: function() {
    return {
      faqArr: faqData,
      currentOpenId: undefined,
    };
  },
  methods: {
    accordionGroupOnClickHandler(id) {
      if (id === this.currentOpenId) {
        this.currentOpenId = undefined;
      } else {
        this.currentOpenId = id;
      }
    },
  },
};
</script>

<style scoped>
#faq {
  position: relative;
  padding-top: 30px;
  padding-bottom: 200px;
}

.faq-content {
  padding: 0 150px;
}

#solarscape {
  position: absolute;
  bottom: 0;
  z-index: -1;
}

#solarscape-panel-dividers,
#solarscape-panels-one,
#solarscape-panels-two {
  opacity: 0.4;
}

[theme='light'] #solarscape-panels-one {
  animation: panel-animation-one 3s linear infinite alternate;
}

[theme='light'] #solarscape-panels-two {
  animation: panel-animation-two 3s linear infinite alternate;
}

@keyframes panel-animation-one {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

@keyframes panel-animation-two {
  0% {
    opacity: 1;
  }

  100% {
    opacity: 0;
  }
}

#solarscape-cloud-one {
  animation: cloud-animation-one 12s linear infinite alternate;
}

#solarscape-cloud-two {
  animation: cloud-animation-two 6s linear infinite alternate;
}

#solarscape-cloud-three {
  animation: cloud-animation-three 8s linear infinite alternate;
}

@keyframes cloud-animation-one {
  100% {
    transform: translateX(24vw);
  }
}

@keyframes cloud-animation-two {
  100% {
    transform: translateX(-12vw);
  }
}

@keyframes cloud-animation-three {
  100% {
    transform: translateX(18vw);
  }
}

@media (--desktop-narrow) {
  .faq-content {
    padding: 0 100px;
  }
}

@media (--mobile-narrow) {
  #faq {
    padding-bottom: 100px;
  }

  .faq-content {
    padding: 0 30px;
  }
}
</style>
