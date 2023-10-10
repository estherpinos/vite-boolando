<script >


export default{
  name:'Header',
  
}

</script>


<template>
  <header class="top-bar-fix">
     <div class="container" id="container-header">

      <!-- MENU -->

      <nav class="menu">
          <ul>
            <li>Donna</li>
            <li>Uomo</li>
            <li>Bambini</li>
          </ul>
        </nav>

        <!-- LOGO BOOLEAN -->

        <div class="logo-bar">
          <img id="boolando-logo" src="../assets/img/boolean-logo.png" alt="boolando-logo">

        </div>

        <!-- MENU ICON -->

        <div class="menu " id="menu-icon-bar">
          <nav class="menu">
            <ul>
              <li class="icon-bar"><i class="fa-regular fa-user"></i></li>
              <li><i class="fa-regular fa-heart"></i></li>
              <li><i class="fa-solid fa-bag-shopping"></i></li>
            </ul>

          </nav>
        </div>
      </div>
  

  </header>
</template>

<style lang="scss" scoped>

@use '../sass/partials/variabiles' as *;

header{
  background-color: $orange-color;
  z-index: 999;
  position: fixed;
  box-shadow: 0 0 10px 0 gray;
  width: 100%;
  height: 60px;
  top: 0;
  left: 0;

  div{
    display: flex;
    justify-content: space-between;
    height: 100%;
    align-items: center;

    nav{
      ul{
        align-items: center;
        li{
          list-style: none;
          color: white;
          font-weight: bold;
          display: inline-block;
          cursor: pointer; 
          padding-left: 10px; 
          

        }
      }
    }
    }

  
  
}




</style>