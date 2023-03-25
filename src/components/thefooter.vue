<template>
    <div>
        <div class="thefooter ">
   <div class="text1 w-100 d-flex  align-items-center justify-content-between p-4">
   <h2 class="fs-1 fw-bolder text-light">Festava Live</h2>
   <div class="iconss d-flex align-item-center gap-5">
    <i class="fa-brands fa-facebook fs-3 text-light"></i>
        <i class="fa-brands fa-instagram fs-3 text-light"></i>
        <i class="fa-brands fa-twitter fs-3 text-light"></i>
        <i class="fa-brands fa-youtube fs-3 text-light"></i>
   </div>
   </div>
   <div class="mainbox p-5 bg-dark">
   <div class="row text-light text-center">
   <div class="col-xl-4 col-lg-4 col-md-4">
    <h3>links</h3>
    <div class="navss d-flex  align-items-center justify-content-between">
     <span>home</span>
     <span>about</span>
     <span>artist</span>
     <span>pricing</span>
     <span>contact</span>
    </div>
   </div>
   <div class="col-xl-4 col-lg-4 col-md-4">
    <h3>Have a question?</h3>
       <p>01021189596</p>
       <p>khaledsawada1@gmail.com</p>
   </div>
   <div class="col-xl-4 col-lg-4 col-md-4">
    <h3>Location</h3>
   <p>cairo , egypt</p>
   <span class="maps">our maps</span>
   </div>
   </div>
   <hr>
   <div class="creat text-center">
    <h3 class="text-light fw-bolder fs-4">created by <span class="text-warning">khaled sawada</span></h3>
   </div>
   
   </div>
  
  </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss">
@import '../sass/main.scss';

.thefooter{
  .text1{
    background-color: $second;
    .iconss{
      i{
        cursor: pointer;
        transition: 0.4s;
        padding: 10px;
        border-radius: 50%;
        &:hover{
          background-color: $primary;
          animation: rot 2s linear infinite;
        }
      }
    }
  }
  .row{
    h3{
      color: $primary;
      font-size: 24px;
      font-weight: bolder;
    }
    p{
      font-size: 17px;
      color: #ccc;
    }
    .maps{
      font-weight: bold;
      text-decoration:underline;
      cursor: pointer;
    }
    .navss{
      span{
        cursor: pointer;
        transition: 0.5s;
        &:hover{
          color:  $link-hover-color;
        }
      }
    }
  }
}


@media(max-width: 500px){
    .thefooter{
    .text1{
      flex-direction: column;
      gap: 30px;
    }
    .row{
      gap: 35px;
    }
  }
}

</style>