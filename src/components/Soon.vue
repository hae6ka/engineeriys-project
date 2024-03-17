<template>
  <section class="soon">
    <h1 class="soon__title">
        {{ title }}
    </h1>
  </section>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Soon",
  props: {
    title: String,
  },
};
</script>

<style scoped lang="scss">
.soon {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #555B85;
    width: 80%;
    height: 300px;
    border-radius: 30px;

    .soon__title {
        font-size: 40px;
        font-weight: 800;
        color: #fff;
    }
}
</style>
