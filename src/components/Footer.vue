<script >

import { menuOptions, menuFooterIcons } from '../data/menuFooter';

export default{
  name:'Footer',
  data(){
    return{  
      menuOptions,
      menuFooterIcons}
  } 
  
}

</script>

<template>
   <footer>
    <section class="section-footer">
      <div class="container">
        <div class="menu-footer">
          <p class="text-footer">Boolando S.r.l</p>
         <nav>
          <ul>
            <li v-for="(item, index) in menuOptions" :key="index">
              <a :href="item.href">{{ item.text }}</a>
            </li>
            
          </ul>
        </nav>
        </div>
        <div class="social-footer">
          <p class="text-footer">Trovaci anche su</p>
          <nav>
            <ul>
              <li v-for="(item, index) in menuFooterIcons" :key="index">
              <a :href="item.href"><i :class="item.icon"></i></a></li>
             

            </ul>
          </nav>
        </div>
        
      </div>

    </section>
  </footer>
</template>

<style lang="scss" scoped>

 @use '../sass/partials/variabiles' as *;

  .section-footer{
  background-color: $color-footer;
  height: 90px;

   
  }

  .container{
    display: flex;
    justify-content: space-between;
    height: 100%;
    margin: 0 auto;
    padding-top: 30px;
    width: 80%;
    max-width: 1000px;
  }
 
  

  .text-footer{
    top: 5px;
    font-size: 15px;
    font-weight: bold;
    color: white;
  }

  .container ul li{
    text-decoration: none;
    display: inline-block;
    padding-right: 10px;
    color: white;
  }

  .container ul li a{
    text-decoration: none;
    font-size: 12px;
    color: white;
  }

  .social-footer ul li {
    display: inline-block;
    padding-left: 5px;
    text-decoration: none;
    color: white

  }

  .social-footer li a{
    text-decoration: none;
    color: white;
  }
  
</style>