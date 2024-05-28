<template>
  <div class="parent-component">
    <h1>Halo!</h1>
    <p>Ini data dari Child: {{ receivedData }}</p>
    <child-component @send-data="handleData"></child-component>
  </div>
</template>

<script>
import ChildComponent from './ChildComponent.vue';

export default {
  components: {
    ChildComponent
  },
  data() {
    return {
      receivedData: ''
    };
  },
  methods: {
    handleData(data) {
      this.receivedData = data;
    }
  }
};
</script>

<style scoped>
/* Style untuk ParentComponent */
.parent-component {
  border: 1px solid #ccc;
  padding: 20px;
  margin: 20px;
  border-radius: 8px;
  background-color: #f9f9f9;
}
</style>
