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
import Header from './components/shared/Header.vue';
import Footer from './components/shared/Footer.vue';
import Servers from './components/server/Servers.vue';
import ServerStatus from './components/server/ServerStatus.vue';

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
