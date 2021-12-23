<template>
  <div>
    <h1>Hello</h1>
    <p>テスト</p>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>

<style lang="scss" scoped>
// $test: #000;
h1 {
  @include mq() {
    color: red;
  }
  font-family: 'Ubuntu', sans-serif;
  font-size: fz(14);
}
</style>
