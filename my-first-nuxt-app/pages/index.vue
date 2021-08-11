<template>
  <div>
    <!-- <Header /> -->
    <button @click="navigate">to products page</button>
    <button @click="toUsers">to users page</button>
  </div>
</template>

<script>
export default {
  methods: {
    navigate() {
      this.$router.push("/products");
    },
    toUsers() {
      this.$router.push("/users");
    }
  },
  layout: "default"
};
</script>
