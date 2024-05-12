<template>
  <div>
    <ul>
      <li v-for="item in items" :key="item.name">{{ item.name }}</li>
      <p v-if="isLoggedIn">Willkommen zurück!</p>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'MyComponent',
  data() {
    return {
      items: [{name: 'Item 1'}, {name: 'Item 2'}],
      isLoggedIn: true
    };
  }
}
</script>

<style scoped>
/* CSS für deine Komponente */
</style>
