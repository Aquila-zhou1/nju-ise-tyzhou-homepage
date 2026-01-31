<!-- src/components/NavBar.vue -->
<template>
  <header class="navbar">
    <div class="nav-container">
      <a href="#" class="nav-logo">
        {{ logoText }}
      </a>

      <nav class="nav-links">
        <a v-for="link in links" :key="link.id" :href="'#' + link.id">
          {{ link.label }}
        </a>
      </nav>

      <!-- <button class="see-more-btn" @click="goDetail">
        &gt; see more detail
      </button> -->
    </div>
  </header>
</template>

<script setup lang="ts">
import { useRouter } from 'vue-router';

interface NavLink {
  id: string;
  label: string;
}

const props = defineProps<{
  logoText: string;
  links: NavLink[];
}>();

const router = useRouter();

const goDetail = () => {
  router.push({ name: 'Detail' });
};
</script>

<style scoped>
.navbar {
  position: sticky;
  top: 0;
  background-color: #ffffff;
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
  padding: 15px 0;
  z-index: 1000;
  width: 100%;
  border-bottom: 1px solid #f0f0f0;
}

.nav-container {
  max-width: 960px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  padding: 0 20px;
  gap: 16px;
}

.nav-logo {
  font-weight: bold;
  font-size: 1.2em;
  color: #527bbd;
  text-decoration: none;
}

.nav-links {
  display: flex;
  gap: 20px;
  flex: 1;
}

.nav-links a {
  color: #555;
  text-decoration: none;
  font-size: 0.9em;
  position: relative;
  padding-bottom: 2px;
}

.nav-links a::after {
  content: '';
  position: absolute;
  width: 0;
  height: 2px;
  bottom: 0;
  left: 0;
  background-color: #527bbd;
  transition: width 0.3s ease;
}

.nav-links a:hover {
  color: #527bbd;
}

.nav-links a:hover::after {
  width: 100%;
}

.see-more-btn {
  border: none;
  background: #527bbd;
  color: #fff;
  padding: 6px 12px;
  border-radius: 4px;
  font-size: 0.85rem;
  cursor: pointer;
  transition: all 0.2s ease;
  white-space: nowrap;
}

.see-more-btn:hover {
  background: #2a4a8c;
  transform: translateY(-1px);
  box-shadow: 0 2px 6px rgba(0,0,0,0.15);
}

@media (max-width: 768px) {
  .nav-container {
    flex-wrap: wrap;
    justify-content: space-between;
  }

  .nav-links {
    flex-wrap: wrap;
    justify-content: center;
    order: 2;
  }

  .see-more-btn {
    order: 1;
  }
}
</style>
