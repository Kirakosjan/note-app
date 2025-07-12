<template>
    
    <div class="card">
        <div class = "close">
        <CloseButton @click = "$"/>
    </div>
        <p class="title"> {{ props.title }}</p>
        <p class="content">
        {{ props.content }}
        </p>     
        <p class="tvakan">
            {{ props.time }}
        </p>
    </div>
</template>

<style>
.card {
    position: relative;
    width: 200px;
    height: 170px;
    border: 1px;
    color: black;
    background: linear-gradient(114.43deg, rgba(255, 255, 255, 0.6) 4%, rgba(255, 255, 255, 0.1) 100%);
    border-radius: 14px;
    padding: 10px 20px 8px 20px;
}

.title {
  font-weight: 600;
  font-style: 500;
  font-size: 21px;
  line-height: 100%;
  letter-spacing: 0%;
  margin-bottom: 20px;
}

.content{
    font-weight: 400;
  font-size: 18px;
  line-height: 100%;
  letter-spacing: 0%;
  width: 100%;
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-line-clamp: 4;
  overflow: hidden;
  min-height: 20px;
}

.tvakan {
  margin-top: 20px;
  text-align: right;
  color:  #797979;
  font-size: 14px;
}

.close-btn {
    width: 25px;
    height: 25px;
    border-radius: 8px;
    border: 2px solid #fff;
    color: #fff;

}
.close {
    position: absolute;
    top: 8px;
    right: 8px;
    opacity: 0;

}
.card:hover .close {
    opacity: 1;
}
</style>

<script setup>
import CloseButton from './CloseButton.vue';
//  import (props) from './Components/defineProps'
import { defineProps } from 'vue';
const props = defineProps(["title", "content", "time"])
</script>