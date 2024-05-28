<template>
  <div id="app">
    <ParentComponent />
  </div>
</template>

<script>
import ParentComponent from './components/ParentComponent.vue';

export default {
  name: 'App',
  components: {
    ParentComponent
  }
};
</script>

<style>
/* Style untuk elemen utama aplikasi */
#app {
  font-family: Poppins;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

/* Style untuk ParentComponent */
.parent-component {
  border: 1px solid #ccc;
  padding: 20px;
  margin: 20px;
  border-radius: 8px;
  background-color: #f9f9f9;
}

/* Style untuk ChildComponent */
.child-component {
  border: 1px solid #b0c4de;
  padding: 15px;
  margin: 15px;
  border-radius: 6px;
  background-color: #e6f7ff;
}

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
