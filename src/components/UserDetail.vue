<template>
    <div class="component">
      <h3>You may view the user details here</h3>
      <p>Many details...</p>
      <p>User Name: {{ switchName() }}</p>
    </div>
</template>

<script>
export default {
  props: ['name'],
  methods: {
    switchName() {
      return this.name
        .split('')
        .reverse()
        .join('');
    },
  },
};
</script>

<style scoped>
div {
  background-color: lightcoral;
}
</style>
