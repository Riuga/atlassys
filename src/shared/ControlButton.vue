<template>
  <div>
    <slot></slot>
  </div>
</template>

<style scoped>
div {
  border-radius: 50%;
  width: 50px;
  height: 50px;
  padding: 12px;
  cursor: pointer;
  background-color: #F5F7FA;
}

@media screen and (max-width: 800px) {
  div {
    display: none;
  }
}
</style>