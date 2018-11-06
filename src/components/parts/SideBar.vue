<template>
  <div>
    <slide right noOverlay>
      <side-bar-item v-for="(item, index) in list" :key="index" :main="item.main" :sub="item.sub">
      </side-bar-item>
    </slide>
  </div>
</template>

<script>
import {Slide} from 'vue-burger-menu';
import SideBarItem from '@/components/parts/SideBarItem';

const itemList = [
  {
    main: 'home',
    sub: '',
  },
  {
    main: 'games',
    sub: 'play games',
  },
  {
    main: 'company',
    sub: 'about us',
  },
  {
    main: 'contact',
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
