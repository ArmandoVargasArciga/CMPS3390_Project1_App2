<script setup>
import HabitTable from './componets/habitTable.vue';

</script>

<template>
  <div id="app">
    <div id="container">
    <HabitTable />
    </div>
  </div>
</template>

<style>
table{
  width: 40%;
  height: 60%;
  border:1px solid black;
  margin: 50px auto;
}

th, td {
  border: 1px solid black;
  padding: 8px 12px;
  text-align: left;
  background-color: white;
}

#container{
  background-color:  white;
  width: 40%;
  height: 60%;
  border:3px solid black;
  margin: 50px auto;
}

#form {
  display: flex;
  gap: 10px;
  width: 40%;
  justify-content: center;
  margin: 50px auto;
}

input {
  padding: 7px;
  font-size: 16px;
  border: 1px solid black;
  border-radius: 3px;
}

button{
    background-color: #007bff;
    border: black solid 1px;
    color: black;
    cursor: pointer;
    padding: 7px 5px;
    font-size: 16px;
    border-radius: 3px;
}

button:hover{
    background-color: #b4cce6;
}

body{
    background-color: #007bff;
    font-family: Arial Helvetica sans-serif;
}
</style>
