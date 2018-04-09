<template>
  <div class="component">
      <h1>The User Component</h1>
      <p>I'm an awesome user!</p>
      <hr>
      <div class="row">
          <div class="cols-xs-12 col-sm-6">
              <user-detail></user-detail>
          </div>
          <div class="cols-xs-12 col-sm-6">
              <user-edit></user-edit>
          </div>
      </div>
  </div>
</template>

<script>
import userDetail from './UserDetail.vue';
import userEdit from './UserEdit.vue';

export default {
  components: {
    userDetail,
    userEdit,
  },
};
</script>

<style scoped>
div {
  background-color: lightblue;
}
</style>
