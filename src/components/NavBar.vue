<template>
  <div id="nav">
    <router-link to="/">
      <img src="@/assets/sign.svg" height="50px" />
      <h1>Home</h1>
    </router-link>
    <NavButtonBasket />
  </div>
</template>

<script>
// @ is an alias to /src
import NavButtonBasket from "@/components/NavButtonBasket.vue";

export default {
  name: "NavBar",
  components: {
    NavButtonBasket
  }
};
</script>

<style lang="scss" scoped>
#nav {
  position: fixed;
  width: 100%;
  z-index: 1;
  top: 0px;
}
img {
  float: left;
  margin: 5px;
}
h1 {
  line-height: 17px;
  float: left;
}
/*  GO FULL WIDTH BELOW 480 PIXELS */
@media only screen and (max-width: 481px) {
  h1 {
    display: none;
  }
}
</style>
