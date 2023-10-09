<template>
  <div v-if="showBanner" class="popup-banner ">
    <h1>User
hi This Ezhumalai Sanjay Welcome to my portfolio . get this senates popup banner design </h1>
    <button @click="toggleBanner">Close</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showBanner: false,
    };
  },
  methods: {
    toggleBanner() {
      this.showBanner = !this.showBanner;
    },
  },
};
</script>

<style scoped>
.popup-banner {
  /* Your banner styling goes here */
}
</style>
