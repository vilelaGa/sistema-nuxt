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
            <!-- <h6>{{ count }}</h6> -->

            <input
              type="email"
              v-model="login.useremail"
              class="form-control"
              placeholder="Email"
            />
            <br />
            <input
              type="password"
              v-model="login.password"
              class="form-control"
              placeholder="Senha"
            />
            <br />
            <div @click="Login()" class="btn btn-primary">Login</div>
            <!-- <button @click="add()" class="btn btn-primary">+</button>
            <button @click="del()" class="btn btn-primary">-</button>
            <button @click="reset()" class="btn btn-primary">RESET</button> -->
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  nome: 'NextQuadroForms',

  data() {
    return {
      login: {
        useremail: '',
        password: '',
      },
      nome: {
        name: 'Gabriel',
        lastname: 'Vilela',
      },
      count: 0,
    }
  },

  computed: {
    NameUser() {
      return `${this.nome.name} ${this.nome.lastname}`
    },
  },

  watch: {
    count(newValue) {
      if (newValue) {
        console.log(this.count + 6)
      }
    },
  },

  methods: {
    add() {
      this.count++
      // console.log(this.count++)
    },
    del() {
      this.count--
      // console.log(this.count--)
    },
    reset() {
      this.count = 0
    },
    Login() {
      try {
        const { useremail, password } = this.login
        console.log(useremail, password)
      } catch (e) {
        consolo.log(e)
      }
    },
  },
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
