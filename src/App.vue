<template>
  <button @click="test1">a button</button>
  <div @click="test1">a div</div>
</template>

<script>
export default {
  methods: {
    test1() {
      window.open('', '_blank');
    },
  },
};
</script>
