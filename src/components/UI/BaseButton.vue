<template>
  <button :class="mode">
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: ['mode'],
};
</script>

<style scoped>
button {
  padding: 0.75rem 1.5rem;
  font-family: inherit;
  background-color: #4a6572;
  border: 1px solid #4a6572;
  border-radius: 12px;
  color: white;
  cursor: pointer;
}

button:hover,
button:active {
  background-color: #232f34;
  border-color: #232f34;
}

.flat {
  background-color: transparent;
  color: #232f34;
  border: none;
}

.flat:hover,
.flat:active {
  color: #f9aa33;
  background-color: #4a6572;
}
</style>
