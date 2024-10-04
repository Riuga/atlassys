<template>
  <div class="sidebar">
    <img class="logo" src="../assets/Logo.svg" />
    <nav>
      <ul>
        <li v-for="element in elements" :key="element.title" :class="element.class">
          <img class="sidebar-img" :src=element.img alt="">
          {{ element.title }}
        </li>
      </ul>
    </nav>
  </div>
</template>

<script setup>
const elements = [{ title: 'Dashboard', img: '/sidebar/Dashboard.svg' }, { title: 'Transactions', img: '/sidebar/Transactions.svg' },
{ title: 'Accounts', img: '/sidebar/Accounts.svg' }, { title: 'Investments', img: '/sidebar/Investments.svg' },
{ title: 'Credit Cards', img: '/sidebar/creditCards.svg' }, { title: 'Loans', img: '/sidebar/Loans.svg' },
{ title: 'Services', img: '/sidebar/Services.svg' }, { title: 'My Privileges', img: '/sidebar/myPrivileges.svg' },
{ title: 'Setting', img: '/sidebar/Setting.svg', class: 'active' }]
</script>

<style scoped lang="scss">
.logo {
  padding: 2rem 1.5rem 2rem 2.5rem;
}

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

.active {
  color: #1814F3;
  border-left: 5px solid #1814F3;
}

li {
  padding: 1rem 1.5rem 1rem 2.5rem;
  width: 100%;
  border-left: 5px solid transparent;
  font-size: 1.5rem;

  img {
    margin-right: 1rem;
  }
}
</style>