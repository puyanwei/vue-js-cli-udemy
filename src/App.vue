<template>
    <div class="container">
        <app-header></app-header>
        <hr>
        <div class="row">
            <servers></servers>
            <server-status></server-status>
        </div>
        <hr>
        <app-footer></app-footer>
    </div>
</template>

<script>
import Header from './Header.vue';
import Footer from './Footer.vue';
import Servers from './Servers.vue';
import ServerStatus from './ServerStatus.vue';

export default {
  // prettier-ignore
  components: {
    'app-header': Header,
    'app-footer': Footer,
    'servers': Servers,
    'server-status': ServerStatus,
  }
};
</script>

<style>
</style>
