<template>
  <button>click</button>
  <input type="text" />
</template>

<script>
export default {
  mounted() {
    const button = document.querySelector('button');
    const input = document.querySelector('input');
    button.addEventListener('click', () => {
      input.value = 'abc';
      input.select();
      document.execCommand('copy');
    });
  },
};
</script>

<style></style>
