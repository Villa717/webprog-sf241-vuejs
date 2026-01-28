<script setup>
import { ref, onMounted } from 'vue'
import { supabase } from './lib/supabaseClient'

const instruments = ref([])

async function getInstruments() {
  const { data, error } = await supabase
    .from('instruments')
    .select()

  if (error) {
    console.error('Supabase error:', error)
    return
  }

  instruments.value = data
}

onMounted(getInstruments)
</script>

<template>
  <ul v-if="instruments.length">
    <li v-for="i in instruments" :key="i.id">
      {{ i.name }}
    </li>
  </ul>
  <p v-else>No data loaded</p>
</template>
