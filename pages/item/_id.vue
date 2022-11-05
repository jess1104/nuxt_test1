<template>
  <div>
    <h1>商品</h1>
    <hr />
    your item is
    <input @keyup.enter="pushId" v-model="id" type="text" />
    <button @click="pushId">確認</button>
    <!-- 用route去拿params -->
    <div v-if="this.$route.params.id">
      商品id為: {{ this.$route.params.id }}
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      id: "",
    };
  },
  methods: {
    pushId() {
      // console.log(this.$route);
      // console.log(this.id);
      this.$router.push({ params: { id: this.id } });
      this.id = "";
    },
  },
};
</script>