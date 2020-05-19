<template>
  <footer class="page-footer" :class="cor || 'light-blue darken-4'">
    <div class="container">
      <div class="row">
        <div class="col l6 s12">
          <h5 class="white-text">{{logo || 'Site'}}</h5>
          <p class="grey-text text-lighten-4">{{descricao || "Uma descrição"}}</p>
        </div>
        <div class="col l4 offset-l2 s12">
          <h5 class="white-text">Links</h5>
          <ul>
            <slot></slot>
          </ul>
        </div>
      </div>
    </div>
    <div class="footer-copyright">
      <div class="container">
        © {{ '2020-2020' }} Copyright {{ logo || 'Site'}}
        <a class="grey-text text-lighten-4 right" href="#!">More Links</a>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterComponent  ',
  props: ['logo', 'cor', 'descricao', 'ano'],
};
</script>

<style scoped>

</style>
