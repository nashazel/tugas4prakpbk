<template>
  <div class="grandchild-component">
    <h3>Grandchild Component</h3>
    <button @click="triggerEvent">Kirim Data ke Parent</button>
  </div>
</template>

<script>
export default {
  methods: {
    triggerEvent() {
      const data = 'Hello from Grandchild!';
      this.$emit('trigger-event', data);
    }
  }
};
</script>

<style scoped>
/* Style untuk GrandchildComponent */
.grandchild-component {
  border: 1px solid #87cefa;
  padding: 10px;
  margin: 10px;
  border-radius: 4px;
  background-color: #e0ffff;
}

/* Style untuk tombol di GrandchildComponent */
.grandchild-component button {
  padding: 10px 20px;
  border: none;
  border-radius: 4px;
  background-color: #87cefa;
  color: white;
  cursor: pointer;
  font-size: 16px;
}

.grandchild-component button:hover {
  background-color: #00bfff;
}
</style>
