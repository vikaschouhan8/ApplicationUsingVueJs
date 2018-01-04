<template>
    <footer>
      <p v-on:click="changeName()"> {{copyright}} {{title}}</p>
    </footer>
</template>

<script>
export default {
  props: {
    title: {
      type: String
    }
  },
  data () {
    return {
      copyright: 'Copyright 2018 Walkover'
    }
  },
  methods: {
    changeName: function() {
      this.title = "New VueJs title"
    }
  }
}
</script>

<style scoped>
footer{
  background-color: #222;
  padding: 6px
}
p{
  color: lightgreen;
  text-align: center;
}
</style>