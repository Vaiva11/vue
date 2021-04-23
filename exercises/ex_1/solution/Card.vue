<template>
  <div class="card">
    <img v-bind:src="require('@/assets/' + image)">
    <div class='text'>
        {{ name }} {{ 2021 - yearOfBirth }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    image: String,
    name: String,
    yearOfBirth: Number
  }
}
</script>

<style scoped>
.card{
    border: solid gray 1px;
    border-radius: 10px;
    width: 300px;
    height: 400px;
    display: flex;
    text-align: center;
    align-items: center;
    flex-direction: column;
    padding: 20px 10px;
    box-shadow: 10px 10px 10px 10px;
    margin: 20px;
}
.text {
    font-size: 30px;
    font-weight: bold;
    margin-top: 60px;
}
</style>
