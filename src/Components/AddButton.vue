
<template>
 <!-- <button class = "buttons" > + </button> -->
 <button class = "add-bin">+</button>

</template>





<script setup>

</script>

<style scopped>

/* .knopka {
width: 68;
height: 68;
top: 744px;
left: 1175px;
border-width: 3px;
angle: 0 deg;
opacity: 1;
color: #4CCB90;
border: 3px solid #FFFFFF; */
/* } */
.add-bin {
    position: fixed;
    bottom: 100px;
    right: 50px;
    width: 60px;
    height: 60px;
    cursor: pointer;
    background:  #4CCB90;
    color: #fff;
    border-radius: 50px;
    font-size: 50px;
    border: 3px solid #FFFFFF; 
    transition: 0.3s;
}
.add-btn:hover {
    background: #38976b;
    transform: scale(1,2);
}

</style>

