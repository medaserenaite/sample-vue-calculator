<template>
  <div class="calculate">
    <p>{{ count }}</p>
    <button @click="minus">-</button>
    <button @click="plus">+</button>
  </div>
</template>

<script>
export default {
  data() {
    return { count: 0 }
  },

  methods: {
    plus() {
      this.count += 1
    },
    minus() {
      this.count -= 1
    }
  }
}
</script>

<style scoped>
.calculate {
  background-color: rgb(176, 249, 225);
  width: 20%;
  padding: 50px;
  border: 1px solid rgb(162, 162, 162);
  margin: auto auto;
}

  button {
    background-color: lavender;
    border: solid 1px rgb(162, 162, 162);
    border-radius: 25px;
    width: 50px;
    height: 40px;
    margin: 5px;
    box-shadow: 0 6px #999;
  }

  button:hover {
    background-color: rgb(202, 202, 245);
    cursor: pointer;
  }

  button:active {
  transform: translateY(2px);
  box-shadow: 0 5px #666;
}
</style>