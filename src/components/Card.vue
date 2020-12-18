<template>
  <div class="card">
    <div class="card-title" :style="{ backgroundColor: titleBackgroundColor }">
      <h3>{{ title }}</h3>
      <strong> (Preço: R$ {{ price }} | Qtde : {{ amount }}) </strong>
    </div>
    <div class="card-form">
      <input type="number" placeholder="Quantidade"/>
      <button>{{ buttonText }}</button>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true,
    },
    buttonText: {
      type: String,
      required: true,
    },
    titleBackgroundColor: {
      type: String,
      required: true,
    },
    price: {
      type: Number,
      required: true,
    },
    amount: {
      type: Number,
      required: true,
    },
  },
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
  flex:1;
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