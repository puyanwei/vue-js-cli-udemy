<template>
    <div class="container">
        <div class="row">
            <div class="cols-xs-12">
                <app-user></app-user>
            </div>
        </div>
    </div>
</template>

<script>
import appUser from './components/User.vue';

export default {
  components: {
    appUser,
  },
};
</script>

<style>
div.component {
  border: 1px solid black;
  padding: 30px;
}
</style>
