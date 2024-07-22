<template>
  <main>
    <p>{{ count }}</p>
    <button @click="sub">Sub</button>
    <button @click="add">Add</button>
  </main>
</template>

<script>
  export default {
    data() {
      return {
        count: 0,
      }
    },
    methods: {
      add() {
        this.count++;
      },
      sub() {
        this.count < 1 || this.count--;
      },
    },
  };
</script>