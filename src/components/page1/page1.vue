<template>
  <div id="page1">
    <el-row>
      <el-col :span="24"><div class="avatar" />
        <img src="img/Avatar.jpg" style="border-radius:50%; width: 30%; height: 30%;">
      </el-col>
    </el-row>
    <br><br><br>
    <el-row>
      <el-col :span="24"><div class="username"/>
        <span style="font-weight: bolder; font-size: 60px; font-family: 'Arial Hebrew'; ">
        {{name}}
      </span>
      </el-col>
    </el-row>
    <br>
    <el-row>
      <el-col :span="24"><div class="username"/>
        <span style="font-weight: normal; font-size: 20px; font-family: 'Arial Hebrew'; ">
        {{ mortal }}
      </span>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: "pageOne",
  data (){
    return {
      name: "Sun Haoran",
      mortal: "吾生也有涯, 而知也无涯．"
    }
  },
}
</script>

<style scoped>
span{
  color: aliceblue;
}
#page1{
  animation: fadeIn; /* referring directly to the animation's @keyframe declaration */
  animation-duration: 1s; /* don't forget to set a duration! */
}

</style>