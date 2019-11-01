<template>
  <div class="row justify-content-center">
    <div class="col-lg-5 col-md-7">
      <div class="card bg-secondary shadow border-0">
        <div class="card-body px-lg-5 py-lg-5">
          <div class="text-center text-muted mb-4">
            <big>Insira seus dados</big>
          </div>
          <form role="form">
            <base-input
              class="input-group-alternative mb-3"
              placeholder="Nome"
              addon-left-icon="ni ni-hat-3"
              v-model="model.name"
            ></base-input>

            <base-input
              class="input-group-alternative mb-3"
              placeholder="CPF"
              addon-left-icon="ni ni-hat-3"
              v-model="model.cpf"
            ></base-input>

            <base-input
              class="input-group-alternative mb-3"
              placeholder="Telefone"
              addon-left-icon="ni ni-hat-3"
              v-model="model.tel"
            ></base-input>

            <base-input
              class="input-group-alternative mb-3"
              placeholder="Cargo"
              addon-left-icon="ni ni-hat-3"
              v-model="model.cargo"
            ></base-input>
            <hr />
            <base-input
              class="input-group-alternative mb-3"
              placeholder="Email"
              addon-left-icon="ni ni-email-83"
              v-model="model.email"
            ></base-input>

            <base-input
              class="input-group-alternative"
              placeholder="Password"
              type="password"
              addon-left-icon="ni ni-lock-circle-open"
              v-model="model.password"
            ></base-input>
            <div class="text-center">
              <base-button type="primary" class="my-4">Cadastrar</base-button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "register",
  data() {
    return {
      model: {
        name: "",
        cpf: "",
        tel: "",
        cargo: "",
        email: "",
        password: ""
      }
    };
  }
};
</script>
<style>
</style>
