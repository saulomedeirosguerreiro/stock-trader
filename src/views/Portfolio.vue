<template>
  <div class="portfolio">
      <Card title="BMW" buttonText="Vender" titleBackgroundColor="rgb(31, 117, 197)" :price="10" :amount="1"/>
      <Card title="BMW" buttonText="Vender" titleBackgroundColor="rgb(31, 117, 197)" :price="10" :amount="1"/>
      <Card title="BMW" buttonText="Vender" titleBackgroundColor="rgb(31, 117, 197)" :price="10" :amount="1"/>
      <Card title="BMW" buttonText="Vender" titleBackgroundColor="rgb(31, 117, 197)" :price="10" :amount="1"/>
      <Card title="BMW" buttonText="Vender" titleBackgroundColor="rgb(31, 117, 197)" :price="10" :amount="1"/>
      <Card title="BMW" buttonText="Vender" titleBackgroundColor="rgb(31, 117, 197)" :price="10" :amount="1"/>
      <Card title="BMW" buttonText="Vender" titleBackgroundColor="rgb(31, 117, 197)" :price="10" :amount="1"/>
      <Card title="BMW" buttonText="Vender" titleBackgroundColor="rgb(31, 117, 197)" :price="10" :amount="1"/>
      <Card title="BMW" buttonText="Vender" titleBackgroundColor="rgb(31, 117, 197)" :price="10" :amount="1"/>
      <Card title="BMW" buttonText="Vender" titleBackgroundColor="rgb(31, 117, 197)" :price="10" :amount="1"/>
      <Card title="BMW" buttonText="Vender" titleBackgroundColor="rgb(31, 117, 197)" :price="10" :amount="1"/>
      <Card title="BMW" buttonText="Vender" titleBackgroundColor="rgb(31, 117, 197)" :price="10" :amount="1"/>
      <Card title="BMW" buttonText="Vender" titleBackgroundColor="rgb(31, 117, 197)" :price="10" :amount="1"/>
      <Card title="BMW" buttonText="Vender" titleBackgroundColor="rgb(31, 117, 197)" :price="10" :amount="1"/>
      <Card title="BMW" buttonText="Vender" titleBackgroundColor="rgb(31, 117, 197)" :price="10" :amount="1"/>
  </div>
</template>

<script>
import Card from '../components/Card';
export default {
  components:{
      Card
  }
};
</script>

<style  scoped>

    .portfolio{
          display: flex;
          flex-wrap: wrap;
    }
</style>