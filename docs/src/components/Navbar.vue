<script setup>
    import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
    import { faDiscord, faGithub } from '@fortawesome/free-brands-svg-icons'
    import { faMagnifyingGlass } from '@fortawesome/free-solid-svg-icons';
</script>

<template>
  <header class="header-container">
    <nav class="nav">
      <div className="search-container">
        <font-awesome-icon :icon="faMagnifyingGlass" class="search-icon" />
        <p>Search in the documentation...</p>
      </div>

      <a href="/" class="nav-link">Home</a>
      <a href="shop.taxzyyyscripts.xyz" class="nav-link">Store</a>

      <div className="divider"></div>

      <button className="light-button"></button>

      <div className="divider"></div>

      <div className="socials-icons">
        <a href="https://github.com/TaxiMax1" target="_blank">
          <FontAwesomeIcon class="social-icon" id="github-icon" :icon="faGithub" />
        </a>

        <a href="https://discord.gg/5Y8hqr64fJ" target="_blank">
          <FontAwesomeIcon class="social-icon" id="discord-icon" :icon="faDiscord" />
        </a>
      </div>
    </nav>
  </header>
</template>