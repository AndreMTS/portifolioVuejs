<template>
  <div>
    <h1>Seja bem-vindo ao meu portfólio</h1>
    <div>
      <p>Nome: {{ name }}</p>
      <p>E-mail: {{ email }}</p>
      <p>Telefone: {{ phone }}</p>
      <ul>
      <li v-for="skill in skills" :key="skill">{{ skill }}</li>
    </ul>
    </div>    
  </div>
</template>

<script>
export default {
  name: 'HomePage',
  data() {
    return {
        name: 'Andre Matos',
        email: 'andrematos@teste.com',
        phone: '+ 55 (31) 9 9290-7896',
        skills: ['Habilidade 1', 'Habilidade 2', 'Habilidade 3']
    }
  }
}
</script>

<style>
h1 {
  text-align: center;
}
</style>
