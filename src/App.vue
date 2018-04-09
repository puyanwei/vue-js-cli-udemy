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
import appHeader from './components/shared/Header.vue';
import appFooter from './components/shared/Footer.vue';
import Servers from './components/server/Servers.vue';
import ServerStatus from './components/server/ServerStatus.vue';

export default {
  // prettier-ignore
  components: {
    appHeader,
    appFooter,
    Servers,
    ServerStatus,
  }
};
</script>

<style>
</style>
