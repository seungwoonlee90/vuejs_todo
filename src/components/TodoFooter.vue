<template>
  <div class="ClearAllContainer">
      <span class="ClearAllBtn" v-on:click="clearTodo">Clear All</span>
      <div class="footer">
        copyright ethanlee
      </div>
  </div>
</template>

<script>
export default {
  methods: {
    clearTodo: function() {
      this.$emit('clearAll');
    }
  }
}
</script>

<style scoped>
.ClearAllContainer {
  width: 8.5rem;
  height: 50px;
  line-height: 50px;
  background-color: white;
  border-radius: 5px;
  margin: 0 auto;
}
.ClearAllBtn {
  color: #FF0266;
  display: block;
}
.footer {
  color: #000000;
  font-weight: 500;
  margin: 0.5rem 0 1.5rem;
}
</style>