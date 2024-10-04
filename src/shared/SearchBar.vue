<template>
  <input type="text" name="search" placeholder="Search for something">
</template>

<style scoped>
input {
  background-image: url('/public/icons/search-icon.png');
  background-size: 20px 20px;
  background-repeat: no-repeat;
  background-position: 25px 15px;
  border-radius: 25px;

  border: none;
  font-size: 16px;
  background-color: #F5F7FA;
  padding: 16px 60px 16px 43px;
  color: #8BA3CB;
}

input::placeholder {
  color: #8BA3CB;
}
</style>