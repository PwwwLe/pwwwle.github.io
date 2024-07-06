<template>
  <nav>
    <ul>
      <li>
        <router-link to='/'>Home</router-link>
      </li>
      <li>
        <router-link to='/about'>About</router-link>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
};
</script>

<style scoped>
nav {
  background-color: #333;
  padding: 1em;
}

ul {
  list-style: none;
  padding: 0;
}

li {
  display: inline;
  margin-right: 1em;
}

a {
  color: white;
  text-decoration: none;
}
</style>
