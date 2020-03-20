<template>
  <div>
    <h2>v-modelのサンプル</h2>

    <div class="field">
      <label>名前 </label>
      <UiTextInput v-model="text" class="input" />
    </div>

    <p v-if="text">こんにちは、 {{text}} さん！</p>
  </div>
</template>

<script>
import UiTextInput from "./UiTextInput.vue";

export default {
  components: {
    UiTextInput
  },

  data() {
    return {
      text: ""
    };
  }
}
</script>

<style scoped>
.field {
  display: flex;
}

label {
  flex-basis: 100px;
}

.input {
  flex-grow: 1;
}
</style>