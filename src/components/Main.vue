<template>
  <main class="main">
    <h1 class="main__title">Лучший лаунчер по майнкрафту</h1>

    <a href="" class="glow-on-hover main__button">Войти!</a>

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
@import '../styles/colors.scss';

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
    background-color: $yellow;
    border-radius: 70px;
    display: flex;
    justify-content: center;
    align-items: center;
    color: #6b6b6b;
    font-weight: 600;
    font-size: 30px;
    text-decoration: none;
    transition: 0.4s all ease-in-out;

    &:hover {
      background-color: $darkblue1;
      color: #fff;
    }
  }

  .main__reg {
    margin-top: 10px;
    color: #fff;
    text-decoration: none;
    font-weight: 100;
  }
}


//btn!!

  .glow-on-hover {
      width: 220px;
      height: 50px;
      border: none;
      outline: none;
      color: #fff;
      background: #111;
      cursor: pointer;
      position: relative;
      z-index: 0;
      border-radius: 10px;
  }

.glow-on-hover:before {
    content: '';
    background: linear-gradient(45deg, #ff0000, #ff7300, #fffb00, #48ff00, #00ffd5, #002bff, #7a00ff, #ff00c8, #ff0000);
    position: absolute;
    top: -2px;
    left:-2px;
    background-size: 400%;
    z-index: -1;
    filter: blur(5px);
    width: calc(100% + 4px);
    height: calc(100% + 4px);
    animation: glowing 20s linear infinite;
    opacity: 0;
    transition: opacity .3s ease-in-out;
    border-radius: 10px;
}

.glow-on-hover:active {
    color: #000
}

.glow-on-hover:active:after {
    background: transparent;
}

.glow-on-hover:hover:before {
    opacity: 1;
}

.glow-on-hover:after {
    z-index: -1;
    content: '';
    position: absolute;
    width: 100%;
    height: 100%;
    background: #111;
    left: 0;
    top: 0;
    border-radius: 10px;
}

@keyframes glowing {
    0% { background-position: 0 0; }
    50% { background-position: 400% 0; }
    100% { background-position: 0 0; }
}
</style>
