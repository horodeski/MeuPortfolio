<script>
export default {
  props: ["text", "tag"],
};
</script>

<template>
  <span>&lt;{{ tag }}&gt;</span>
  <span class="txt">{{ text }}</span>
  <span>&lt;/{{ tag }}&gt;</span>
</template>

<style scoped lang="scss">
span {
  font-weight: 600;
  font-size: 1.7em;
  color: #29a1d2;
}
.txt {
  color: white;
}
</style>
