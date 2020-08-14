<template>
  <div>
    <MenuBurger />

    <!-- filter black opacity video -->
    <div class="container__filter"></div>

    <MainContainer />
  </div>
</template>

<script>
// @ is an alias to /src
import MainContainer from "@/components/MainContainer";
import MenuBurger from "@/components/MenuBurger";

export default {
  name: "Home",
  components: {
    MainContainer,
    MenuBurger,
  },
};
</script>

<style scoped>
.container__filter {
  position: absolute;
  background-color: rgba(12, 12, 12, 0.5);
  width: 100vw;
  height: 100vh;
  z-index: 10;
}
</style>
