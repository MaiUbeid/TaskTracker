<template>
  <button @click="onClick()" :style="{ background: color }" class="btn">
    {{ text }}
  </button>
  <!-- v-on:click="onClick()" v-bind:style="" -->
</template>

<script>
export default {
  name: "Button",
  props: {
    text: String,
    color: String,
  },
  methods: {
    onClick() {
      this.$emit("btn-click");
    },
  },
};
</script>
