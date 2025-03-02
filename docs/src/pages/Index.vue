<script setup>
const title = 'Welcome'
const description = `Welcome to the Taxzyyy scripts documentation.`
const underdescripion = `Here you will find useful information relating to my scripts.`
</script>

<template>
  <div className="welcome-page">
    <h1>{{ title }}</h1>
    <p>{{ description }}</p>
    <p>{{ underdescripion }}</p>
    <div className="last-update" >{{ `Last updated: 01.03.2025, 15.48` }}</div>
  </div>
</template>