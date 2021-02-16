<template>
  <div class="tab-item" @click="itemclick" >
    <slot v-if="!istrue" name="tab-item-img"></slot>
    <slot v-else name="tab-item-ing"></slot>
      
      
      <div :style="color">
        <slot  name="tab-item-div"></slot>
      </div>
      
     
  </div>
</template>

<script>
export default {
  props:{
    path: String,
    stylecolor:{
      type:String,
      defalut:'blue'
    }
  },
  data(){
    return {
      //  istrue:  true
    }
  },
  computed:{
    istrue(){
      return this.$route.path.includes(this.path) 
      
    },
    color(){
      return this.istrue?{color:this.stylecolor}:{}
    }
  },
  methods:{
    itemclick(){
      this.$router.replace(this.path).catch(()=>{})
    }
  }

}
</script>

<style>
 .tab-item{
    flex: 1;
    text-align: center;
    height: 49px;
    
  }
  .tab-item img{
      width:29px;
      height:29px;
      margin-bottom:-6px;
  }
  
 
</style>