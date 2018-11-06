<template>
  <slide right PushRotate>
    <side-bar-item v-for="(item, index) in list" :key="index" :main="item.main" :sub="item.sub" :state="item.state">
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
    state: 'build',
  },
  {
    main: 'Games',
    sub: 'play games',
    state: 'build',
  },
  {
    main: 'Company',
    sub: 'about us',
    state: 'build',
  },
  {
    main: 'Contact',
    sub: 'send a mail',
    state: 'build',
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
