<template>
  <div id="app">
    <header>
      <AppNavbar></AppNavbar>
    </header>
    <main>
      <router-view/>
    </main>
    <AppFooter>
      <li><a class="grey-text text-lighten-3" href="#!">Link 1</a></li>
      <li><a class="grey-text text-lighten-3" href="#!">Link 2</a></li>
      <li><a class="grey-text text-lighten-3" href="#!">Link 3</a></li>
      <li><a class="grey-text text-lighten-3" href="#!">Link 4</a></li>
    </AppFooter>
  </div>
</template>

<script>
import AppNavbar from './components/layouts/NavbarComponent';
import AppFooter from './components/layouts/FooterComponent';

export default {
  name: 'App',
  components: {
    AppNavbar,
    AppFooter,
  },
};
</script>
