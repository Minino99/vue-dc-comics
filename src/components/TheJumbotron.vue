<template>
  <div>
    <div class="jumbocontainer">
     <div class="jumboimg"><img :src="JumboImg" alt=""></div>
     <div class="floatingbtn container"><button type="button" class="btn btn-primary btn-lg">CURRENT SERIES</button></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheJumbotron",
  props: {
   JumboImg: String,
  }
};
</script>

<style lang="scss" scoped>
.jumbocontainer {
 height: 360px;
}

.jumboimg{
 height: 100%;
 width: 100%;
 background-position: center;
 background-size: cover;
 overflow: hidden;
 img{
   width: 100%;
   transform: translateY(-20%);
 }
}

.floatingbtn{
 transform: translateY(-50%);
}

.btn-primary {
  color: #fff;
  background-color: #0081EF;
  border-color: #0081EF;
  border-radius: 0;
  font-weight: 700;
  font-size: 1.7rem;
}

</style>
