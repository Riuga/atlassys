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
  margin-left: 16%;
}
</style>
