<template>
<div id="whole" @wheel="handleScroll">

  <img id="up" src="img/up.png" class="image" style="width: 5%; height: 5%;margin-bottom: 10%">

  <div id="page1"><page-one ></page-one></div>


  <img id="down" src="img/down.png" class="image" style="width: 5%; height: 5%;margin-top: 10%">

  <div id="page2"><page-two ></page-two></div>


</div>
</template>

<script>
import 'animate.css';
import PageOne from "@/components/page1/page1";
import PageTwo from "@/components/page2/page2";
export default {
  name: "cardAvatar",
  components: {PageTwo, PageOne},
  methods: {
    handleScroll(e) {
      if (e.deltaY > 0) {
        // 向下滚动...
        var t =document.getElementById("page1")
        t.style.display = "none"
        var x =document.getElementById("page2")
        x.style.display = "block"
        var d =document.getElementById("down")
        d.style.display = "none"
        var u =document.getElementById("up")
        u.style.display = "inline"
      } else {
        // 向上滚动...
        var a =document.getElementById("page1")
        a.style.display = "block"
        var b =document.getElementById("page2")
        b.style.display = "none"
        var c =document.getElementById("down")
        c.style.display = "inline"
        var f =document.getElementById("up")
        f.style.display = "none"
      }
    }
  }
}
</script>

<style scoped>
span{
  color: aliceblue;
}

#page2{
  display: none;
  animation: fadeIn; /* referring directly to the animation's @keyframe declaration */
  animation-duration: 1s; /* don't forget to set a duration! */
  color: aliceblue;
  margin-left: 10%;
}

#down{
  animation: fadeInUp; /* referring directly to the animation's @keyframe declaration */
  animation-duration: 1s; /* don't forget to set a duration! */
  display: inline;
}
#up{
  display: none;
  animation: fadeInDown; /* referring directly to the animation's @keyframe declaration */
  animation-duration: 1s; /* don't forget to set a duration! */
}

#leftCol{
  /**/
}
#rightCol{
  margin-right: 50%;
  font-size: 30px;
}
</style>