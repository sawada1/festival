<template>
    <div>
        <header class="site-header p-3">
                <div class="container">
                    <div class="row">
                        
                        <div class="col-lg-12 col-12 d-flex flex-wrap ">
                            <p class="d-flex mb-0 align-items-center gap-2">
                              <i class="fa-solid fa-user"></i>
                                <strong class="text-dark fw-bolder fs-6">Welcome to Music Festival 2023</strong>
                            </p>
                        </div>

                    </div>
                </div>
            </header>
            <nav class="navbar navbar-expand-lg  " :class="{'active':check}">
                <div class="container">
                <router-link to="/" style="text-decoration: none;">
                  <h1 class="navbar-brand  fs-sm-1 fs-2 fw-bolder " style="color:#fff" >
                        Festava Live
                    </h1>
                </router-link>
                   

                    <!-- <a href="" class="">Buy Ticket</a> -->
                    <router-link to="/about" style="text-decoration: none;">
                          <button class="btn custom-btn thebtnn d-lg-none d-sm-none d-md-block ms-auto me-4">Buy Ticket</button>                        
                        </router-link>
    
                    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                        <span class="navbar-toggler-icon"></span>
                    </button>
    
                    <div class="collapse navbar-collapse" id="navbarNav">
                        <ul class="navbar-nav align-items-lg-center ms-auto me-lg-5">
                            <li class="nav-item">
                            <router-link to="/" @click="check2 = 1" class="nav-link click-scroll" :class="{'active':check2 == 1}" href="#landing">
                              Home                            
                            </router-link>
                            </li>
    
                            <li class="nav-item">
                                <a @click=" check2 = 2" class="nav-link click-scroll" :class="{'active':check2 == 2}" href="#about">About</a>
                            </li>
    
                            <li class="nav-item">
                                <a @click="check2 = 3" class="nav-link click-scroll" :class="{'active':check2 == 3}" href="#artist">Artists</a>
                            </li>

                            <li class="nav-item">
                                <a @click="check2 = 4" class="nav-link click-scroll" :class="{'active':check2 == 4}" href="#Schedule">Schedule</a>
                            </li>

                            <li class="nav-item">
                                <a @click="check2 = 5" :class="{'active':check2 == 5}" class="nav-link click-scroll" href="#Pricing">Pricing</a>
                            </li>
    
                            <li class="nav-item">
                                <a @click=" check2 = 6" class="nav-link click-scroll" :class="{'active':check2 == 6}" href="#contact">Contact</a>
                            </li>
                        </ul>

                        <router-link to="/about" style="text-decoration: none;">
                          <button class="btn thebtnn   d-lg-block d-none">Buy Ticket</button>                        
                        </router-link>

                    </div>
                </div>
            </nav>
        
    </div>
</template>

<script>
import {ref} from 'vue'
export default {
  setup(){
    let check = ref(false);
    let check2 = ref(1);
    const scrolling = ()=>{
      window.addEventListener("scroll",()=>{
        if(window.scrollY >= 50){
        //  console.log('scrolll');
        check.value = true
        } else if(window.scrollY == 0 ){
          check.value = false
        }
      });
    }
       scrolling();

    return{check, check2}
  }

}

</script>

<style lang="scss">
@import '../sass/main.scss';
.site-header{
  background-color: $primary;
  i{
    color:$second;
    font-size: 20px;
  }
}
.navbar{
background-color: transparent;
 z-index: 1111;
 transition: 0.5s;
 background-color: gray;
 a{
  color: #fff;
  transform: 0.5s;
 }
 &.active{
  background-color: #333;
  position: fixed;
   top: 0px;
 left: 0;
 right: 0;
 transition: 0.5s;
 }

 .collapse {
  background-color: transparent;
  a{
    transition: 0.5s;
    &:hover, &.active{
      color: $second;
    }
  }
 }
}

</style>