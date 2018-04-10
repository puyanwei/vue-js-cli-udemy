<template>
  <div class="component">
      <h1>The User Component</h1>
      <p>I'm an awesome user!</p>
      <button @click="changeName">Change My Name</button>
      <hr>
      <p>The name is {{ name }}</p>
      <hr>
      <div class="row">
          <div class="cols-xs-12 col-sm-6">
              <user-detail
              :myName="name"
              @nameWasReset="name = $event"
              :resetFn="resetName"
              :userAge="age"
              ></user-detail>
          </div>
          <div class="cols-xs-12 col-sm-6">
              <user-edit
              :userAge="age"
              @ageWasEdited="age = $event"
              ></user-edit>
          </div>
      </div>
  </div>
</template>

<script>
import userDetail from './UserDetail.vue';
import userEdit from './UserEdit.vue';

export default {
  data: function() {
    return {
      name: 'Ken',
      age: 27,
    };
  },
  methods: {
    changeName() {
      this.name = 'Ryu';
    },
    resetName() {
      this.name = 'Ken';
    },
  },
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
