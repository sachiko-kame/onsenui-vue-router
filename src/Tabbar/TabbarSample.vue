<template>
  <v-ons-page>
    <v-ons-toolbar>
      <div class="left" v-if="$options.name === 'Home'"></div>
      <div class="left" v-else>
        <v-ons-back-button>Back</v-ons-back-button>
      </div>
    </v-ons-toolbar>
    <v-ons-tabbar position="auto"
      :tabs="tabs"
      :visible="true"
      :index.sync="activeIndex"
    ></v-ons-tabbar>
  </v-ons-page>
</template>

<script>
import tabOne from './Tab/TabOne.vue';
import tabTwo from './Tab/TabTwo.vue';
import tabThree from './Tab/TabThree.vue';

export default {
  data() {
    return {
      activeIndex: 0,
      tabs: [
        {
          label: 'One',
          page: tabOne
        },
        {
          label: 'Two',
          page: tabTwo,
        },
        {
          label: 'Three',
          page: tabThree
        }
      ]
    }
  }
}
</script>