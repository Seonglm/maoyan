<template>
  <div>
    <van-nav-bar :title="title" left-arrow @click-left="onClickLeft" />
  </div>
</template>

<script>
export default {
  methods: {
    onClickLeft() {
      this.$router.go(-1);
    },
    download() {
      this.$router.push("/download");
    }
  },
  props: {
    title: String,
    flag: {
      type: Boolean,
      default: true
    }
  }
};
</script>

<style lang="scss" scoped>
.van-nav-bar {
  background: #e54847;
  height: 1.5625rem;
  line-height: 1.5625rem;
}

.van-nav-bar,
.van-icon {
  color: #fff;
  font-size: 0.8125rem;
}

.van-nav-bar__title {
  color: #fff;
  font-size: 0.5625rem;
}
</style>
