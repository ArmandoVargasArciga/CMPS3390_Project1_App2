<script setup>
 function test(){

 }
</script>

<template>
<table>
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
  <button @click="test">TEST</button>
</table>
</template>

<style scoped>
table{
  width: 40%;
  border:1px solid black;
  margin: 50px auto;
}
</style>
