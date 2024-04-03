<template>
  <footer class="footer">creatED by Мамкин программист, dev-mode</footer>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Footer",
  props: {},
};
</script>

<style scoped lang="scss">
@import "../styles/colors.scss";

.footer {
  margin-top: 30px;
  color: #fff;
  font-weight: 100;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 50px;
  background-color: $darkblue1;
}
</style>