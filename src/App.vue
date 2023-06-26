<template>
  <img class="back" alt="Dijon" src="./assets/back.webp" />
  <div class="content">
    <img alt="Marmelab logo" src="./assets/logo-moutarde.png" />
    <TitleMessage msg="Gildas, on arrive, met la moutarde au frais !!!" />
    <CountDown deadline="2023-06-28T15:20:00.000Z" />
    <div id="greenframe_embedable_score_page"></div>
  </div>
</template>

<script>
import TitleMessage from "./components/TitleMessage.vue";
import CountDown from "./components/CountDown.vue";

export default {
  name: "App",
  components: {
    TitleMessage,
    CountDown,
  },
};
</script>
<script
  id="greenframe_embedable_score_page_script"
  src="https://cc7b-81-250-164-94.ngrok-free.app/embedable_score_page.js"
  size="big"
></script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  padding-top: 60px;
}

@media (max-width: 1250px) {
  #app {
    padding-top: 10px;
  }
}

.back {
  width: calc(100% - 60px);
  margin: 30px;
  position: absolute;
  top: 0;
  left: 0;
  filter: contrast(40%) blur(5px) brightness(1.5);
}

@media (max-width: 1250px) {
  .back {
    margin: -10px;
    height: calc(100% + 20px);
    width: unset;
  }
}

.content {
  position: relative;
}

#greenframe_embedable_score_page {
  position: absolute;
  bottom: 10px;
  right: 40px;
}
</style>
