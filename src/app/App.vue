<template>
  <SideBar />
  <div class="content">
    <Header />
    <Profile />
  </div>
</template>

<script setup>
import Header from '../widgets/Header.vue'
import SideBar from '../widgets/SideBar.vue'
import Profile from '../widgets/Profile.vue'
</script>

<style scoped>
.content {
  position: relative;
  margin-left: 16vw;
}

@media screen and (max-width: 1200px) {
  .content {
    margin-left: 10vw;
  }
}

@media screen and (max-width: 800px) {
  .content {
    margin-left: auto;
  }
}
</style>
