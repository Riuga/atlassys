<template>
  <header>
    <img class="sidebar-btn" src="../assets/sidebar.svg" alt="sidebar" />
    <h1>Setting</h1>
    <SearchBar />
    <ControlButton>
      <img class="control" src="../assets/setting.svg" alt="settings">
    </ControlButton>
    <ControlButton>
      <img class="control" src="../assets/notification.svg" alt="notification">
    </ControlButton>
    <img class="avatar" src="../assets/avatar.jpg" alt="avatar">
  </header>
</template>

<script setup>
import SearchBar from '../shared/SearchBar.vue';
import ControlButton from '../shared/ControlButton.vue';

</script>

<style lang="scss">
header {
  height: 100%;
  display: flex;
  justify-content: space-between;
  height: 100px;
  padding: 2rem 1.5rem 2rem 2.5rem;
  align-items: center;
  text-align: center;
  background-color: #fff;

  .sidebar-btn {
    display: none;
    width: 1rem;
  }

  h1 {
    margin-right: auto;
  }

  .avatar {
    width: 60px;
    height: 60px;
    border-radius: 50%;
  }

  * {
    margin-right: 1rem;
  }

}

@media screen and (max-width: 800px) {
  header {
    flex-wrap: wrap;
    height: 200%;

    .sidebar-btn {
      display: inline;
    }

    h1 {
      margin: 0 auto;
    }

    .control {
      display: none;
    }

    input {
      order: 1;
      width: 100%;
    }
  }
}
</style>