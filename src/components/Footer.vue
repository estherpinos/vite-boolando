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
      <div class="container-footer">
        <div class="menu-footer">
          <p class="text-footer">Boolando S.r.l</p>
        <nav>
          <ul>
            <li v-for="item in menuOptions">
              <a :href="item.href">{{ item.text }}</a>
            </li>
            
          </ul>
        </nav>
        </div>
        <div class="social-footer">
          <p class="text-footer">Trovaci anche su</p>
          <nav>
            <ul>
              <li v-for="item in menuFooterIcons">
              <a :href="item.href"><i :class="item.icon"></i></a></li>
             

            </ul>
          </nav>
        </div>
        
      </div>

    </section>
  </footer>
</template>

<style>
  .section-footer{
  background-color: #1A1A1A;
  height: 90px;
}

.container-footer{
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

.container-footer ul li{
  text-decoration: none;
  display: inline-block;
  padding-right: 10px;
  font-size: 12px;
  color: white;
}

.text-footer li a{
  text-decoration: none;
  color: white;
}

.social-footer li a{
  padding-left: 5px;
  text-decoration: none;
  color: white;

}
</style>