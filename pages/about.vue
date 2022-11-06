<template>
  <div>
    <h1>bootstrap 按鈕</h1>
    <hr />
    <div>
      <b-button>BButton</b-button>
      <b-button variant="danger" @click="alert">紅色警戒</b-button>
      <b-button variant="success">綠色和平</b-button>
      <a
        href="https://www.tiktok.com/@6467hu/video/7148322160543681818?is_copy_url=1&is_from_webapp=v1"
        ><b-button variant="primary">藍色妖姬</b-button></a
      >
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    alert() {
      alert("警告");
    },
  },
};
</script>