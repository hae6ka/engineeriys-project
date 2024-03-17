<template>
  <main class="main">
    <h1 class="main__title">Лучший лаунчер по майнкрафту</h1>

    <a href="" class="main__button">Войти!</a>

    <a class="main__reg" href="/reg"> Нет акка? Регайся! </a>
  </main>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Main",
};
</script>

<style scoped lang="scss">
.main {
  max-width: 950px;
  width: 80%;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  align-items: center;

  .main__title {
    font-size: 50px;
    font-weight: 700;
    color: #fff;
  }

  .main__button {
    margin-top: 50px;
    width: 300px;
    height: 60px;
    background-color: #f9b17a;
    border-radius: 70px;
    display: flex;
    justify-content: center;
    align-items: center;
    color: #6b6b6b;
    font-weight: 600;
    font-size: 30px;
    text-decoration: none;
  }

  .main__reg {
    margin-top: 10px;
    color: #fff;
    text-decoration: none;
    font-weight: 100;
  }
}
</style>
