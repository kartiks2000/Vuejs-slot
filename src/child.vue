<template>
  <div>
    <h1>Hello!! I am the first child....</h1>
    <h2>my name is kartik .</h2>
    <slot></slot>
  </div>
</template>

<script>
import {mybus} from './main';
export default {
    props:{
        age : Number,
    },
    methods:{
        changing(){
            this.age = 19;
            mybus.$emit("agechanging",19);
        }
    }
}
</script>

<style scoped>
    h1{
        color: blue;
    }
    div{
        background-color: burlywood;
        padding: 2rem;
    }
</style>

