<template>
  <div class="row justify-content-center">
    <div class="col-lg-5 col-md-7">
      <div class="card bg-secondary shadow border-0">
        <div class="card-body px-lg-5 py-lg-5">
          <div class="text-center text-muted mb-4">
            <big>Entrar</big>
          </div>
          <form role="form">
            <base-input
              class="input-group-alternative mb-3"
              placeholder="Email"
              addon-left-icon="ni ni-email-83"
              v-model="model.email"
            ></base-input>

            <base-input
              class="input-group-alternative"
              placeholder="Senha"
              type="password"
              addon-left-icon="ni ni-lock-circle-open"
              v-model="model.password"
            ></base-input>

            <!-- <base-checkbox class="custom-control-alternative">
              <span class="text-muted">Remember me</span>
            </base-checkbox>-->
            <div class="text-center">
              <base-button type="primary" class="my-4">Entrar</base-button>
            </div>
          </form>
        </div>
      </div>
      <div class="row mt-3">
        <div class="col-12 text-center">
          <router-link to="/register" class="text-primary">
            <p>Create new account</p>
          </router-link>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "login",
  data() {
    return {
      model: {
        email: "",
        password: ""
      }
    };
  }
};
</script>
<style>
</style>
