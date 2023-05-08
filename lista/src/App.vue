<script setup>

'São Paulo',
    'Rio de Janeiro',
    'Belo Horizonte',
    'Salvador',
    'Fortaleza',
    'Curitiba',
    'Manaus',
    'Recife',
    'Porto Alegre',
    'Brasília'

    const cidades = [
        { id: 1, name: 'Rio de Janeiro', details: { description: 'Rio de Janeiro description', estado: "Rio de Janeiro" } },
        { id: 2, name: 'Belo Horizonte', details: { description: 'Belo Horizonte description', estado: "Minas gerais" } },
        { id: 2, name: 'Salvador', details: { description: 'Belo Horizonte description', estado: "Minas gerais" } },
        { id: 2, name: 'Fortaleza', details: { description: 'Belo Horizonte description', estado: "Minas gerais" } },
        { id: 2, name: 'Curitiba', details: { description: 'Belo Horizonte description', estado: "Minas gerais" } },
        { id: 2, name: 'Belo Horizonte', details: { description: 'Belo Horizonte description', estado: "Minas gerais" } },
        { id: 2, name: 'Belo Horizonte', details: { description: 'Belo Horizonte description', estado: "Minas gerais" } },
    ]
</script>
<template>
  <ul>
    <li v-for="item in items" :key="item.id">
      <p>Nome: {{ item.name }}</p>
      <p>Detalhes</p>
      <p v-for="(value, key) in item.details" :key="key">{{ key }}: {{ value }}</p>
    </li>
  </ul>
</template>