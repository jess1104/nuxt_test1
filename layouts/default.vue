<template>
  <div>
    <header>
      <h1>Jess網站</h1>
      <NuxtLink class="nav" to="/">Home</NuxtLink> ||
      <NuxtLink class="nav" to="/about">about</NuxtLink> ||
      <NuxtLink class="nav" to="/article/list">article(list)頁</NuxtLink>
      <NuxtLink class="nav" to="/item">item頁</NuxtLink>
    </header>
    <Nuxt />
  </div>
</template>

<script>
export default {
  name: "default",

  created() {
    this.getDogImage();
  },
  methods: {
    getDogImage() {
      const api = `https://dog.ceo/api/breeds/image/random`;
      this.$axios.get(api).then((respons) => {
        console.log(respons);
        // this.image = respons.data.message;
      });
    },
  },
};
</script>

<style scoped>
.nav {
  display: inline-block;
  margin-left: 10px;
}
</style>