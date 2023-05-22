<script>
export default {
  props: {
    menuItems: Array,
  },
};
</script>

<template>
  <ul class="nav">
    <li v-for="items in menuItems" :key="items.title">{{ items.title }}</li>
  </ul>
</template>

<style lang="scss" scoped>
.nav {
  display: flex;
  gap: 1rem;
  list-style: none;
}

.nav li {
  cursor: pointer;
  font-size: 1.1em;
  font-weight: bold;
  position: relative;
  margin-top: 44px;
  padding-inline: 0.3rem;
  padding-top: 5px;
  &:hover {
    background-color: rgba(2, 130, 249, 0.3);
  }
}

// CLASSE ACTIVE GIà PRONTA NEL CASO IN CUI SI DIA LOGICA ALL'ELEMENTO (C'è ANCHE IL TRATTINO SOTTO IL FIGLIO ATTIVO)

// .nav li.active {
//   color: #0282f9;
//   &::after {
//     content: "";
//     display: block;
//     width: 45px;
//     height: 9px;
//     background-color: #0282f9;
//     position: absolute;
//     top: 66px;
//     left: 12px;
//   }
// }
</style>
