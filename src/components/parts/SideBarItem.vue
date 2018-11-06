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
div {
  @import url('https://fonts.googleapis.com/css?family=Varela+Round');

  font-family: 'Varela Round', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
}
.container {
  height: 70px;
  display: block;
  border-bottom: solid 1px #3d332a;

  color: white;
  &:hover {
    color: khaki;
  }
}
.main-text {
  font-size: 35px;
}
.sub-text {
  font-size: 20px;
}
</style>
