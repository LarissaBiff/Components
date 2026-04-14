<script setup>
    defineProps(['nome', 'tipo', 'acao'])
</script>


<template>
    <button :class="[tipo, acao]">
        {{ nome }}
    </button>
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
</style>