<template>
  <div class="container">
    <div class="main-text">
      {{main}}
    </div>
    <div class="sub-text">
      {{sub}}
    </div>
  </div>
</template>

<script>
export default {
  props: {
    main: {
      type: String,
      require: true,
      default: '',
    },
    sub: {
      type: String,
      require: false,
      default: '',
    },
  },
};
</script>

<style lang="scss" scoped>
.container {
  height: 70px;
}
.main-text {
  font-size: 14px;
}
.sub-text {
  font-size: 10px;
}
</style>
