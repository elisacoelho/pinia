<script setup> 
import { ref }  from 'vue';
import { useCounterStore } from '@/stores/counter';

const CounterStore = useCounterStore()
</script>

<template>
  <div class="about">
    <h1>This is an about page</h1>
  <h2>Contador: {{ CounterStore.count }}</h2>
  <h2>Dobro do Contador: {{ CounterStore.doubleCount }}</h2>
    <button @click="CounterStore.increment">+</button>
</div>  
</template>

<style scoped>
</style>