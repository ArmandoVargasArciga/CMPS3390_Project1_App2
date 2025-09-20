<script setup>

</script>

<template>
<table>
  <tr>Habit List</tr>
  <tr>
    <th>Hobby</th>
    <th>Date</th>
  </tr>
  <tr>
    <td>Essay due</td>
    <td>9/20/2025</td>
  </tr>
  <tr>
    <td>Birthday</td>
    <td>9/25/2025</td>
  </tr>
  <input type="text">
  <button @click="test">TEST</button>
</table>
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