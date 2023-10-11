<script >

import menuMain from '../data/menuMain';


export default{
  name:'Main',
 data(){
  menuMain

 }
  
  
}

</script>

<template>
 <main>
  <div class="container" id="container-main">
        <div class="product">
          <img src="../assets/img/1.webp" alt="1-wwb">
          <span class="saldi">-50%</span>
          <span class="sostenibilità">Sostenibilità</span>
          <div class="product-2">
            <img src="../assets/img/1b.webp" alt="1-b-web">
          </div>
          <div class="heart"><i class="fa-solid fa-heart"></i></div>


          <div class="text-foto">
            <p class="marca">Levi´s</p>
            <h4>RELAXED FIT TEE UNISEX</h4>
            <span class="prezzo-saldi">14,99 &euro;</span>
            <span class="prezzo">29,99 &euro;</span>

          </div>
        </div>

  </div>
 </main>
 
 
</template>

<style lang="scss" scoped>
@use '../sass/partials/variabiles' as * ;

#container-main{
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  margin: 100px auto;
  width: 80%;
}

.product{
  position: relative;
}

.product img{
  width: 300px;
  margin: 8px;
}

.product-2{
  position: absolute;
  top: 0;
  left: 0;
  opacity: 0;
  transition: 0.5s;
}

.product:hover .product-2{
  opacity: 1;
} 

/* TEXT PREZZO E MARCA */

.text-foto{
  padding-left: 8px;
  margin-bottom: 40px;
}

.marca{
  font-size: 15px;
  font-weight: lighter;
  color: rgba(0, 0, 0, 0.616);
  
}

.product h6{
  font-weight: bold;
  font-size: 20px;
 
}

.prezzo-saldi{
  color: red;
  font-size: 15px;
  font-weight: lighter;
  
}

.prezzo{
  text-decoration: line-through;
  font-size: 15px;
  font-weight: lighter;
  color: rgba(0, 0, 0, 0.616);
}

/* BOX PREZZO */

.saldi{
  position: absolute;
  top: 370px;
  z-index: 10;
  left: 8px;
  background-color: red;
  color: white;
  font-size: 10px;
  padding: 5px 8px;
}

.sostenibilità{
  position: absolute;
  top: 370px;
  z-index: 10;
  left: 48px;
  background-color: #007E00;
  color: white;
  font-size: 10px;
  padding: 5px 8px;
}

.heart{
  position: absolute;
  z-index: 90;
  top: 20px;
  right: 9px;
  background-color: white;
  padding: 10px 10px;
}

 .heart:hover {
  color: red;
}
</style>