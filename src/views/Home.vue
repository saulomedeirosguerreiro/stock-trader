<template>
  <div class="home">
    <div class="info">
      <h1>Negocie e Consulte suas Ações</h1>
      <p class="paragraph blue">
        <i class="fas fa-info-circle"></i>Você pode Salvar &amp; Carregar os
        Dados
      </p>
      <p class="paragraph green">
        <i class="fas fa-info-circle"></i>Clique em 'Finalizar Dia' para iniciar
        um novo dia !
      </p>
    </div>
    <div class="info-balance">
        <span>Seu Saldo: R$ 10.000</span>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.home {
  margin-left: 100px;
}

.home h1 {
  text-align: left;
}

.info-balance{
    width:91%;
    text-align: left;
    border-top: 1px solid gray;
}

.info-balance span{
    font-size: 1.3rem;
    font-weight: 400;
}

.paragraph {
  max-width: 90%;
  text-align: left;
  padding: 10px;
  color: white;
}

.green {
  background: rgb(63, 167, 63);
}
.blue {
  background: rgb(31, 117, 197);
}

p i {
  margin: 0 5px;
}
</style>