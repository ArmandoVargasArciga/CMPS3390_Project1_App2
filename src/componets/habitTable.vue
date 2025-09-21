<script setup>
import { ref } from 'vue'

const newHabit = ref('')
const habits = ref([])

function addHabit() {
  if (!newHabit.value.trim()) {
    alert('Please enter a habit.')
    return
  }

  const today = new Date().toLocaleDateString()

  habits.value.push({
    name: newHabit.value.trim(),
    date: today
  })

  newHabit.value = ''
}
</script>

<template>
<table>
  <tr>Habit List</tr>
  <tr>
    <th>Habit</th>
    <th>Date</th>
  </tr>

    <tr v-for="(habit, index) in habits" :key="index">
      <td>{{ habit.name }}</td>
      <td>{{ habit.date }}</td>
    </tr>
  
</table>
<div id="form">
  <input v-model="newHabit">
  <button @click="addHabit">Add</button>
</div>


</template>

<style scoped>
table{
  width: 40%;
  height: 60%;
  border:1px solid black;
  margin: 50px auto;
}
th{
  border:1px solid black;
}
</style>