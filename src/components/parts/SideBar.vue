<template>
  <slide right PushRotate>
    <side-bar-item v-for="(item, index) in list" :key="index" :main="item.main" :sub="item.sub">
    </side-bar-item>
  </slide>
</template>

<script>
import {Slide} from 'vue-burger-menu';
import SideBarItem from '@/components/parts/SideBarItem';

const itemList = [
  {
    main: 'Home',
    sub: 'go to home',
  },
  {
    main: 'Games',
    sub: 'play games',
  },
  {
    main: 'Company',
    sub: 'about us',
  },
  {
    main: 'Contact',
    sub: 'send a mail',
  },
];

export default {
  data() {
    return {
      list: [],
    };
  },
  mounted() {
    this.list = itemList;
  },
  components: {
    Slide,
    SideBarItem,
  },
};
</script>

<style lang="scss" scoped>
.slide-bar {
  width: 400px;
}
</style>
