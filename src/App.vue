<template>
  <Header />
  <Paintings />
</template>

<script>
import Header from "./components/HeaderComp.vue";
import Paintings from "./components/PaintingsComp.vue";

export default {
  components: {
    Header,
    Paintings,
  },
};
</script>
