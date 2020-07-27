<template>
  <div>
    <!-- 页面顶部 -->
    <header>
      <div class="nav-header">{{ this.$route.name }}</div>
    </header>
  </div>
</template>

<script>
export default {
  methods: {
    download() {
      this.$router.push("/download");
    }
  },
  props: {
    scrollTop: Number
  }
};
</script>

<style lang="scss" scoped>
header {
  z-index: 1;
  background: #fff;
  width: 100%;
  .nav-header {
    height: 1.5625rem;
    background: #e54847;
    color: #fff;
    text-align: center;
    line-height: 1.5625rem;
    font-size: 0.5625rem;
  }
}
</style>
