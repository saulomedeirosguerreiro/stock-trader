<template>
     <header>
      <div class="menu-left">
        <ul>
          <span><strong>STOCK</strong>TRADER</span>
          <li><a href="/">INÍCIO</a></li>
          <li><a href="/portfolio">PORTIFÓLIO</a></li>
          <li><a href="/actions">AÇÕES</a></li>
        </ul>
      </div>
      <div class="menu-right">
         <ul>
          <li><a href="#home">FINALIZAR DIA</a></li>
          <li><a href="#news">SALVAR &amp; CARREGAR</a></li>
          <li><span>Saldo: R$ 10.000</span></li>
        </ul>
      </div>
    </header>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
header{
  display: flex;
  justify-content: space-between;
  background: #f3f3f3;
  border-bottom: 2px solid  #d3d3d3;
  box-shadow: 0 10px 5px grey;
}

li{
   list-style-type: none;
   display: inline;
   margin: 0 10px;
}

li span{
    color: gray;
}

a{
  text-decoration: none;
  color: #424242;
  font-weight: 400;
}

a:hover{
  color: #d3d3d3;
}
</style>