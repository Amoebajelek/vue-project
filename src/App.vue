<template>
  <HeaderComp @changeTitle="ubahText" :text="text" />
</template>

<script>
import HeaderComp from '@/components/Header-Comp.vue'
export default {
  name: 'App',
  components: {
    HeaderComp
  },
  data(){
    return{
      text: "ini adalah text dari App.vue",
    }
  },
  methods: {
    ubahText(newText){
      this.text = newText
    }
  }
}
</script>

<style>

</style>
