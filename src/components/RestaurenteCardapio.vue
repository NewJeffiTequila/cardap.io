<template>
  <div>
        <div class="d-flex justify-content-center mb-3">
            <h1>Nome do Restaurante</h1>
            <img class="" src="@/assets/logo2.png" alt="" width="50px">
        </div>
        <div class="d-flex justify-content-center mb-3">
            <b-button v-b-modal.modal-pratos>Pratos</b-button>
            <b-button v-b-modal.modal-bebidas>Bebidas</b-button>

            <b-modal id="modal-pratos" hide-footer title="Selecione os Pratos e as Quantidades">
                <ModelPratos/>

            </b-modal>

            <b-modal id="modal-2" title="Cardapio de Bebidas">
                <p class="my-4">Hello from modal2!</p>
            </b-modal>
        </div>
            
    
  </div>
</template>

<script>

import ModelPratos from './ModelPratos'
export default {
    components:{
        ModelPratos
    },

}
</script>

<style>
    #modal-2{
        background-color:#4682B4;
    }
</style>