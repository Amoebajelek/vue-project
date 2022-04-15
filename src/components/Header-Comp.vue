<template>
  <h3>VueJs dan {{ text }} </h3>
  <button @click="changeText">Ubah Text</button>
</template>

<script>
export default {
  name: "HeaderComp",
  props: ["text"],
  data(){
    return{
      newText: "ini adalah text dari header.vue"
    }
  },
  methods: {
    changeText(){
      this.$emit("changeTitle", this.newText)
    }
  },
  emits: ["changeTitle"]
};
</script>

<style></style>
