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

<style scoped>
.nav {
  margin-left: 10px;
}
</style>