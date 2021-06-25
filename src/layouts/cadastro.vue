<template>
  <main>
        <div class="row">
            <div class="col-lg-6 fundoPrimario">
                <!--Imagem de Fundo-->
            </div>

            <!--Início Formulário-->
            <div class="col-lg-6 d-flex fundoSecundario">
                <div class="container align-self-center d-flex justify-content-center">
                    <form class="d-flex justify-content-center">
                        <div class="align-self-center">
                            <h1 class="display-5 pb-2">Cadastre -se</h1>
                            <p class="lead pb-4">Seja bem vindo (a)!</p>
                            <div>
                                <input class="mb-4" type="text" placeholder="Digite seu nome" />
                            </div>
                            <div>
                                <input class="mb-4" type="email" placeholder="Digite seu email" />
                            </div>
                            <div>
                                <input type="password" placeholder="Digite sua senha" />
                            </div>
                            <button type="button" class="btn btn-primary mt-4">Entrar</button>
                            <p class="text-center pt-3">
                                <!--<a routerLink="/login">Já possui acesso? <b>Entrar</b></a>-->
                                <router-link to="/login">
                                    <a>Já possui acesso? <b>Entrar</b></a>
                                </router-link>
                            </p>
                        </div>
                    </form>
                </div>
            </div>
            <!--Final Formulário-->
        </div>
    </main>

</template>


<style>
    * {
  padding: 0;
  margin: 0;
  overflow-x: hidden;
}

/*Imagem de fundo*/

main .fundoPrimario {
  background: url('../assets/fundo.png');
  background-repeat: no-repeat;
  background-position: center;
  height: 640px;
}


main .fundoSecundario {
  background-color: #03345f;
}


/*Formulário*/

main form {
  border: 1px solid #fff;
  border-radius: 8px;
  -webkit-border-radius: 8px;
  -moz-border-radius: 8px;
  height: 450px;
  width: 350px;
  color: #fff;
}


main form input {
  border: 1px solid #fff;
  height: 40px;
  width: 300px;
  border-radius: 4px;
  -webkit-border-radius: 4px;
  -moz-border-radius: 4px;
}


main form input::-webkit-input-placeholder {
  color: #000;
}


main form .btn-primary,
main form .btn-primary:hover {
  background-color: #051f2e;
  border: none;
}


main form button {
  width: 300px;
  height: 40px;
}


main form a {
  text-decoration: none;
  color: #fff;
}

main form a:hover {
  text-decoration: underline;
  color: #fff;
}



/*Portrait phones, less than 579px*/
@media (max-width: 575.98px) {
  main .fundoPrimario {
      height: 250px;
      background-size: cover;
      background-position: top center;
  }

  main form {
      margin: 40px 0px 40px 0px;
      height: 430px;
  }
}


/*Tablets, 768px and up*/
@media (min-width: 768px) and (max-width: 991.98px) {
  main .fundoPrimario {
      height: 400px;
      background-position: top center;
  }

  main form {
      margin: 40px 0px 40px 0px;
      height: 430px;
  }
}

</style>

<script>
  export default {
    name: 'cadastro',
    data() {
      return {}
    }
  }
</script>
