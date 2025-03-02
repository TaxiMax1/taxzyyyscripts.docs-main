<script setup>
import tslogo from '../assets/tslogo.png';

import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
import { faAngleRight } from '@fortawesome/free-solid-svg-icons';
import { ref } from 'vue';

const activeButton = ref('');

const setActiveButton = (buttonLabel) => {
  activeButton.value = buttonLabel;
};

const links = [
  { label: "Home", href: "/" },
  { label: "Dashboard", href: "/dashboard" },
  { label: "Settings", href: "/settings" },
  { label: "Help", href: "/help" }
];
</script>

<template>
  <aside class="sidebar-container">
    <nav class="sidebar-nav">
      <div class="nav-header">
        <img :src="tslogo" class="logo" />
        <p class="brand-name">Taxzyyy Scripts</p>
      </div>

      <div class="divider2"></div>
      <div class="realbatman"></div>

      <div
        class="link-button"
        :class="{ active: activeButton === 'Introduction' }"
        @click="setActiveButton('Introduction')"
      >
        <div class="link-buttons">
          Introduction
        </div>
      </div>

      <div
        class="link-button"
        :class="{ active: activeButton === 'Guides' }"
        @click="setActiveButton('Guides')"
      >
        <div class="link-buttons">
          Guides
          <font-awesome-icon :icon="faAngleRight" class="icon-dropdown" />
        </div>
      </div>
    </nav>
  </aside>
</template>