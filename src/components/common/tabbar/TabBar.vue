<template>
  <div id="tabbar">
      <slot></slot>
  </div>
</template>

<script>
export default {

}
</script>

<style>
#tabbar{
    display:flex;
    background-color:pink;
    position: fixed;
    left: 0;
    right:0;
    bottom: 0;
    box-shadow: 0 -2px 3px rgba(100,100, 100, 0.6);
   

  }
 
</style>