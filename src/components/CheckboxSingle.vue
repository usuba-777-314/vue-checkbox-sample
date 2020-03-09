<template>
  <div>
    <h2>単体のチェックボックス</h2>

    <input type="checkbox" id="checkbox" v-model="checked">
    <label for="checkbox">{{ checked }}</label>
  </div>
</template>

<script>
export default {
  data() {
    return {
      checked: false
    };
  }
};
</script>
