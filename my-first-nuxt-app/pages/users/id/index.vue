<template>
  <div>
    <h1>A Single User with ID {{ $route.params.id }}</h1>
    <nuxt-link to="/users">Users</nuxt-link>
    <userItem :name="$route.params.id" />
  </div>
</template>

<script>
import userItem from "../../../components/userItem.vue";
export default {
  component: {
    userItem
  },
  validate(data) {
    console.log(data);
    return true;
  }
};
</script>

<style></style>
