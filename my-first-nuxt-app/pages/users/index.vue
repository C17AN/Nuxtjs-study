<template>
  <div>
    <p>The Users View ({{ userId }})</p>
    <input
      :value="userId"
      placeholder="유저명을 입력하세요"
      @input="changeName"
    />
    <button @click="printName">유저 이름 출력!</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userId: "Chanmin"
    };
  },
  methods: {
    changeName(e) {
      this.userId = e.target.value;
    },
    printName() {
      alert(this.userId);
      this.$router.push("/users/" + this.userId);
    }
  }
};
</script>

<style></style>
