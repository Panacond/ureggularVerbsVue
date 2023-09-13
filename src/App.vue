<script setup>
import RowHead from './components/RowHead.vue'
import RowWord from './components/RowWord.vue'
import wordsJson from './words.json'
import Back from './components/Back.vue'
</script>

<template>
  <RowHead/>
  <RowWord v-for="(i, index) in wordsJson" :word="i" :index="index"/>
  <Back  :wordsJson="wordsJson"/>
</template>