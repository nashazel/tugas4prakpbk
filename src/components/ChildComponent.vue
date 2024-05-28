<template>
  <div class="child-component">
    <h2>Child Component</h2>
    <grandchild-component @trigger-event="sendDataToParent"></grandchild-component>
  </div>
</template>

<script>
import GrandchildComponent from './GrandchildComponent.vue';

export default {
  components: {
    GrandchildComponent
  },
  methods: {
    sendDataToParent(data) {
      this.$emit('send-data', data);
    }
  }
};
</script>

<style scoped>
/* Style untuk ChildComponent */
.child-component {
  border: 1px solid #b0c4de;
  padding: 15px;
  margin: 15px;
  border-radius: 6px;
  background-color: #e6f7ff;
}
</style>
