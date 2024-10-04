<template>
  <header>
    <h1>Setting</h1>
    <div class="controls">
      <SearchBar />
      <ControlButton>
        <img src="../assets/setting.svg" alt="settings">
      </ControlButton>
      <ControlButton>
        <img src="../assets/notification.svg" alt="notification">
      </ControlButton>
      <img class="avatar" src="../assets/avatar.jpg" alt="avatar">
    </div>
  </header>
</template>

<script setup>
import SearchBar from '../shared/SearchBar.vue';
import ControlButton from '../shared/ControlButton.vue';

</script>

<style lang="scss">
header {
  display: flex;
  justify-content: space-between;
  height: 100px;
  padding: 2rem 1.5rem 2rem 2.5rem;
  align-items: center;
  text-align: center;
  background-color: #fff;

  .controls {
    display: flex;
    justify-content: space-between;
    width: 33%;

    .avatar {
      width: 60px;
      height: 60px;
      border-radius: 50%;
    }

  }
}
</style>