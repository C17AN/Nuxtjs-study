<template>
  <div>
    <button @click="navigate">to products page</button>
  </div>
</template>

<script>
import Header from "../components/Header.vue";
export default {
  components: {
    Header
  },
  methods: {
    navigate() {
      this.$router.push("/products");
    }
  }
};
</script>
