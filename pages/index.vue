<template>
    <div class="two2">
      <app-navbar/>
      <div class="two">
        <div class="grid">
          <div class="two1">
           <h2>Do more than what is expected of you with HAMLET.</h2>
           <p>Great leaders know their strengths, but they know their weaknesses even better. Knowing when to act
              and when to step back is one of the skills a leader must master.
            </p>
            <nuxt-link to='/signin'> <button class="btn1">Sign In <img src="/img/Polygon 1.png" alt=""></button></nuxt-link>
            <nuxt-link to='/signup'> <button  class="btn2">Get started <img src="/img/Polygon 1.png" alt=""></button></nuxt-link>
          </div>
          <div>

          </div>
        </div>
      </div>
    </div>
</template>


<script>
import Navbar from '~/components/navbar2.vue';
export default {
    components:{
      'app-navbar': Navbar
    }
}
</script>


<style scoped>
    .two{
      background:linear-gradient(to right, rgba(8, 29, 41, 0.7),
       rgba(8, 29, 41, 0.7)), url('/img/nesa.jpg') no-repeat center center/cover ;
       height: 120vh;
       margin-top: 4rem;
       
    }
    .grid{
      padding:15rem 100px ;
      display: grid;
      grid-template-columns: 1fr 1fr;
      text-align: left;
    }
    .two1 h2{
      color: #FFFFFF;
      font-size: 45px;
      margin-bottom: 20px;
    }
    .two1 p{
      color: #FFFFFF;
      font-size: 25px;
      margin-bottom: 20px;
    }
    .btn2{
      background: #0065FC;
      border-radius: 5px;
      color: white;
      padding: 10px 20px;
      border: none;
      outline: none !important;
    }
    .btn1{
      background: white;
      color: #0065FC;
      border-radius: 5px;
      padding: 10px 20px;
      border: none;
      margin-right: 30px;
      outline: none !important;
    }
    

    @media(max-width:567px){
      .two{
      background:linear-gradient(to right, rgba(8, 29, 41, 0.7),
       rgba(8, 29, 41, 0.7)), url('/img/nesa.jpg') no-repeat center center/cover ;
       height: auto;
       
    }
      .grid{
      padding:8rem 20px ;
      grid-template-columns: 1fr ;
    }
      .two1 h2{
      color: #FFFFFF;
      font-size: 40px;
      margin-bottom: 26px;
    }
    .two1 p{
      color: #FFFFFF;
      font-size: 20px;
      margin-bottom: 26px;
    }
    }


    @media (min-width:568px) and (max-width:768px){

      .two{
      background:linear-gradient(to right, rgba(8, 29, 41, 0.7),
       rgba(8, 29, 41, 0.7)), url('/img/nesa.jpg') no-repeat center center/cover ;
       height: auto;
       
    }
      .grid{
      padding:10rem 20px ;
      grid-template-columns: 1fr 1fr;
      text-align: justify;
    }
      .two1 h2{
      color: #FFFFFF;
      font-size: 40px;
      margin-bottom: 26px;
    }
    .two1 p{
      color: #FFFFFF;
      font-size: 20px;
      margin-bottom: 26px;
    }
    }

    @media (min-width:769px) and (max-width:1200px){
        .two{
      background:linear-gradient(to right, rgba(8, 29, 41, 0.7),
       rgba(8, 29, 41, 0.7)), url('/img/nesa.jpg') no-repeat center center/cover ;
       height: auto;
       
    }
      .grid{
      padding:10rem 20px ;
      grid-template-columns: 1fr 1fr;
      text-align: justify;
      margin-left: 80px;
    }
    .two1 h2{
      color: #FFFFFF;
      font-size: 3rem;
      margin-bottom: 30px;
    }
    .two1 p{
      color: #FFFFFF;
      font-size: 20px;
      margin-bottom: 30px;
    }
    }


    
</style>