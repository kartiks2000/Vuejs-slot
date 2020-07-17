<template>
  <div class="kk">
    <h1>Hello!! I am the parent....</h1>
    <Child>
      <h1>how are you???</h1>
      </h2>i am {{post}}</h2>
    </Child>
  </div>
</template>

<script>
import child from './child';
export default {
  components:{
    Child : child,
  },
  data:() => {
    return {
      post : "product manager"
    }
  }
}
</script>

<style scoped>
  h1{
    color: red;
  }
  div{
    margin: 3rem;
  }
  .kk{
    background-color: cornsilk;
    padding: 3rem;
  }
</style>>
