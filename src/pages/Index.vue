<template>
  <q-page class="column justify-center items-center">
   <div class="row items-center justify-around q-mt-xl container-logo">
     <q-img src="../assets/logo-white.png" width="55px" />
      <strong>Alysson</strong>
   </div>
   <q-icon name="keyboard_arrow_down" size="28px" class="q-icon-arrow"/>
   <q-card class="my-card q-ma-lg" flat bordered>
     <q-card-section horizontal class="q-pa-lg">
        <div class="container-card">
          <q-icon name="payment" size="35px" class="q-icon-card"></q-icon>
          <div class="info-container q-mt-xl">
            <strong class="text-uppercase">Fatura Atual</strong>
            <h4 class="q-ma-none">R$ 1.254,40</h4>
            <div>
              <span>Limite disponível:</span>
              <strong class="q-ml-sm text-uppercase">RS 1.000.500,00</strong>
            </div>
          </div>
        </div>
        <q-card-actions vertical class="column justify-center">
          <div class="div-orange"></div>
          <div class="div-blue"></div>
          <div class="div-green"></div>
        </q-card-actions>
     </q-card-section>
     <div class="bottom-container row items-center justify-between q-pa-sm q-mb-md q-mx-sm ">
      <q-icon size="25px" name="fastfood"></q-icon>
      <span class="q-mx-sm">Compra mais recente em Minha Delicia no valor de R$50,00</span>
      <q-icon size="20px" name="keyboard_arrow_right" />
     </div>
   </q-card>

  </q-page>
</template>

<script>
export default {
  name: 'PageIndex'
}
</script>

<style lang="scss">
  .container-logo {
    width: 45%;
    strong{
      color: $white;
      font-size: 22px;
    }
  }
  .q-icon-arrow{
    color: $white;
    
  }
  .my-card {
    width: 80%;
    max-width: 330px;
    height: 340px;
  }
  .container-card{
    width: 95%;
  }
  .q-icon-card{
    color: $grey;
  }
  .info-container{
    height: 100px;
    h4 {
      color: $blue;
      font-weight: bold;
    }
    strong:first-child{
      color: $blue;
    }
    span{
      color: $grey;
    }
    strong{
      color: $green;
    }
  }
  .div-orange{
    height: 30px; 
    width: 7px;
    background-color: $orange;
    border-top-left-radius: 5px;
    border-top-right-radius: 5px;
  }
  .div-blue{
    height: 70px; 
    width: 8px;
    background-color: $blue;
  }
  .div-green{
    height: 105px; 
    width: 7px;
    background-color: $green;
    border-bottom-left-radius: 5px;
    border-bottom-right-radius: 5px;
  }
  .bottom-container{
    .q-icon{
      color: $grey;
    }
    span{
      color: $grey;
      width: 75%;
    }

  }
  .card-items{
    height:140px;
    widht:115px;
    background-color: $darkPurple;
    color: $white;
    cursor: pointer;
  }
  .q-scrollarea{
    width: 95%;
    height:145px;
  }

</style>