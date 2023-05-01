<script>
export default {
  props: ["text"],
};
</script>

<template>
  <h2><span>&lt;h2&gt;</span>{{ text }}<span>&lt;/h2&gt;</span></h2>
</template>

<style scoped lang="scss">
span {
  font-weight: 600;
  color: #29a1d2;
}
</style>
