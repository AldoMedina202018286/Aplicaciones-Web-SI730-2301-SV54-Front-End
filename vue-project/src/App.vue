<script setup>
    import HelloWorld from './components/HelloWorld.vue'
    import ListComponent from "@/components/list-component.vue";
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />
  </header>
  <nav>
    <router-link to="/">Go to Home</router-link>
    <router-link to="/AddTutorial/:id">Go to add Tutorial</router-link>
    <router-link to="/ListComponent">Go to list Component</router-link>

  </nav>
  <main>
      <router-view />
  </main>
  <footer>
      <div>Footer</div>
  </footer>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
