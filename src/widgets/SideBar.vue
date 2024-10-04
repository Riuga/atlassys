<template>
  <div class="sidebar">
    <img src="../assets/Logo.svg" />
    <nav>
      <ul>
        <li v-for="element in elements" :key="element.title">
          <img class="sidebar-img" :src=element.img alt="">
          {{ element.title }}
        </li>
      </ul>
    </nav>
  </div>
</template>

<script setup>
import SideBarElement from '../shared/SideBarElement.vue'

const elements = [{ title: 'Dashboard', img: '/sidebar/Dashboard.svg' }, { title: 'Transactions', img: '/sidebar/Transactions.svg' },
{ title: 'Accounts', img: '/sidebar/Accounts.svg' }, { title: 'Investments', img: '/sidebar/Investments.svg' },
{ title: 'Credit Cards', img: '/sidebar/creditCards.svg' }, { title: 'Loans', img: '/sidebar/Loans.svg' },
{ title: 'Services', img: '/sidebar/Services.svg' }, { title: 'My Privileges', img: '/sidebar/myPrivileges.svg' },
{ title: 'Setting', img: '/sidebar/Setting.svg' }]
</script>

<style scoped>
.sidebar {
  position: fixed;
  height: 100vh;
  z-index: 2;
  background-color: #FFF;
  width: 16%;
}

.sidebar-img {
  width: 25px;
  height: 25px;
}
</style>