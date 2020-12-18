<template>
  <div class ="card">
    <div class="card-title" :style="{ backgroundColor: titleBackgroundColor }">
      <h3>{{ title }}</h3>
      <strong>
        (Preço: R$ {{ item.price }}
        <template v-if="showAmount">| Qtde : {{ item.amount }} </template> )</strong
      >
    </div>
    <div class="card-form">
      <input type="number" placeholder="Quantidade" v-model.number="amount" />
      <button @click="clickButton">{{buttonText}}</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      amount: 0,
    };
  },
  computed:{
      showAmount(){
          return !!this.item.amount && this.buttonText === 'Vender'
      }
  },
  props: {
    title: {
      type: String,
      required: true,
    },
    titleBackgroundColor: {
      type: String,
      required: true,
    },
    buttonText: String,
    item: {
      type: Object,
      required: true,
    }
  },
  methods:{
      clickButton(){
          const {item, amount} = this
          this.$emit('click', {item, amount})
          this.amount = 0
      } 
  }
};
</script>

<style scoped>
.card {
  width: 30vw;
  color: white;
  text-align: left;
  box-shadow: 2px 2px 5px gray;
  margin: 10px;
}

.card-form {
  display: flex;
  align-items: center;
  height: 120px;
  border: 1px solid gray;
}

.card-form input {
  flex: 1;
  height: fit-content;
  border: 0;
  margin: 0 10px;
  padding: 10px 25px;
  border-bottom: 1px solid gray;
  outline: none;
}

.card-form button {
  height: fit-content;
  margin-right: 20px;

  background-color: #d3d3d3;
  border: none;
  padding: 10px 25px;
  text-align: center;
  font-size: 16px;
  cursor: pointer;
}

.card-title {
  display: flex;
  align-items: center;
  padding: 5px;
}

.card-title strong {
  font-size: 1.3rem;
}

.card-title h3 {
  display: inline;
  margin: 0 10px;
}
</style>