<template>
  <div>
    <h1>Articles</h1>
    <router-link
      :to="{
        name: 'Article',
      }"
      >Link to article</router-link
    >
  </div>
</template>
<script lang="ts">
import { defineComponent, onMounted } from "vue";

export default defineComponent({
  name: "Articles",
  setup() {
    onMounted(() => {
      console.log("--- ARTICLES MOUNTED ---");
    });
  },
});
</script>
