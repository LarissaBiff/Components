<script setup>
  import buttonChild from './components/buttonChild.vue';
</script>


<template>
  <div class="container">
      <div>
        <button class="btn btn-novo">Novo</button>
        <button class="btn btn-editar">Editar</button>
        <button class="btn btn-salvar">Salvar</button>
        <button class="btn btn-cancelar">Cancelar</button>
        <button class="btn btn-excluir">Excluir</button>
      </div>
      <div>
        <buttonChild :nome="'Novo'" :tipo="'btn'" :acao="'btn-novo'"> Novo </buttonChild>
      </div>
  </div>
</template>


<style scoped>

.btn {
  background-color: rgb(179, 46, 68);
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  margin: 5px;
  font-weight: bolder;
}
.btn-novo {
  background-color: white;
  color: rgb(179, 46, 68);
}
.btn-editar {
  background-color: rgb(179, 77, 46);
  color:  white;
}
.btn-salvar {
  background-color:  rgb(50, 138, 57); 
  color: white;
}
.btn-cancelar {
  background-color:  rgb(46, 48, 179);
  color: white;
}
.btn-excluir {
  background-color: rgb(179, 46, 68);
  color:  white;
}
.btn button {
  cursor: pointer;

}
</style>
