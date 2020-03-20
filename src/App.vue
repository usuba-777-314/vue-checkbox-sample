<template>
  <div id="app">
    <h1>チェックボックスのサンプル</h1>

    <div class="content">
      <CheckboxSingle />
      <CheckboxMultiple />
    </div>

    <div class="content">
      <TextInput />
    </div>
  </div>
</template>

<script>
import CheckboxSingle from './components/CheckboxSingle.vue'
import CheckboxMultiple from './components/CheckboxMultiple.vue'
import TextInput from './components/TextInput.vue'

export default {
  name: 'App',
  components: {
    CheckboxSingle,
    CheckboxMultiple,
    TextInput
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  display: flex;
  flex-direction: column;

  width: 600px;
  margin: 60px auto 0;

  text-align: left;
  color: #2c3e50;
}
</style>
