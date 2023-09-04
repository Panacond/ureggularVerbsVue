<script setup>
import RowHead from './components/RowHead.vue'
import RowWord from './components/RowWord.vue'
import wordsJson from './words.json'
</script>

<template>
  <RowHead/>
  <RowWord v-for="i in wordsJson" :word="i"/>
</template>

