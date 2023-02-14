<template>
  <div class="login">
    <div class="quadro">
      <div class="container">
        <div class="row">
          <div class="p-4 mt-4">
            <Logo />
          </div>
        </div>
        <div class="row">
          <div class="p-4 mt-3">
            <span>Bem-vindo ao Dashboard</span>
            <h6>Entre na sua conta</h6>

            <input type="email" class="form-control" placeholder="Email" />
            <br />
            <input type="password" class="form-control" placeholder="Senha" />
            <br />
            <button class="btn btn-primary">Login</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  nome: 'NextQuadroForms',
}
</script>

<style>
.quadro {
  background: #292929;
  width: 300px;
  height: 430px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.quadro h6,
span {
  color: #f0f0f0;
}
</style>
