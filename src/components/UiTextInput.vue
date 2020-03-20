<template>
  <input v-model="text" class="ui-text-input" placeholder="入力してください">
</template>

<script>
export default {
  props: {
    value: {
      type: String
    }
  },

  computed: {
    text: {
      get() {
        return this.value;
      },
      set(text) {
        this.$emit("input", text);
      }
    }
  }
}
</script>

<style scoped>
.ui-text-input {
  display: block;
  border-width:0px;
  border-style:None; 
  font-size: 18px;
  background-color: rgba(0,0,0,0);
  outline: 0;

  border-bottom: 1px solid #d0d0d0;
}
</style>
