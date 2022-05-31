<template>
  <button @click="test1">a button</button>
  <div @click="test1">a div</div>
</template>

<script>
export default {
  methods: {
    test1() {
      fetch('https://jsonplaceholder.typicode.com/todos/1')
        .then((response) => response.json())
        .then((json) => console.log(json));
      window.open('', '_blank');
    },
  },
};
</script>
