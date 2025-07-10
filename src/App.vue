<script setup>
import Card from './Components/Card.vue' 
import AddButton from './Components/AddButton.vue';
</script>

<style>
body {
  width: 100%;
  height: 100%;
}


main.main {
  background: linear-gradient(128deg, rgba(135, 246, 180, 0.84) 12.75%, rgba(50, 180, 187, 0.67) 83.4%);

  width: 100%;
  min-height: 100vh;

}

h1 {

  color: black;
  text-align: center;
  padding: 24px;


}

.notes {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    gap: 26px;
    flex-wrap: wrap;
    justify-content: center;
}
</style>



<template>
  <main class="main">
    <h1>Note App</h1>
    <!-- <Card /> -->
      <div class = "notes">
    <Card />
    <Card />
    <Card />
    <Card />
    <Card />
    <Card />
    <Card />
    </div>

    <AddButton/>
  </main>

</template>