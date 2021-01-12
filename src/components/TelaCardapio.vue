<template>
    <div>
        <div class="d-flex justify-content-center mb-3">
            <img src="@/assets/hamburger-solid.svg" alt="" width="60">
            <h1 class="display-4">CARDAP.IO</h1>
        </div>
        <div class=" justify-content-center col-sm-2 ">
            <b-form>
                <b-form-group
                    id="input-group-1"
                    label="Email do Restaurante:"
                    label-for="input-1"
                >
                    <b-form-input
                        id="input-1"
                        type="email"
                        placeholder="Digite seu Email"
                        required
                    >
                    </b-form-input>
                </b-form-group>
                <b-form-group id="input-group-1" label="Senha:" label-for="input-1">
                    <b-form-input type="password" id="text-password" aria-describedby="password-help-block"></b-form-input>
                </b-form-group>

               
            </b-form>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>

</style>