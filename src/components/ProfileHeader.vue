<!-- src/components/ProfileHeader.vue -->
<template>
  <section class="profile-container">
    <div class="profile-info">
      <h1>{{ name }}</h1>
      <h3>{{ title }}</h3>
      <p>
        <a href="https://ise.nju.edu.cn/en/index.htm" target="_blank">
          School of Intelligent Software and Engineering
        </a><br />
        <a href="http://www.nju.edu.cn/" target="_blank">
          Nanjing University, Suzhou Campus, China
        </a><br /><br />
        Email:
        <a href="mailto:liwenbin@nju.edu.cn">tyzhou@smail.nju.edu.cn</a>
        <br /><br />
        <span class="social-links">
          <a class="social-link" href="https://github.com/Aquila-zhou1" target="_blank">GitHub</a>
        </span>
      </p>
    </div>

    <div class="profile-image">
      <img :src="photoSrc" 
      :alt="name" 
      @error="(e) => console.log('当前尝试加载的实际值是: ' + photoSrc)"
      class="profile-photo" />
    </div>
  </section>
</template>

<script setup lang="ts">
const props = defineProps<{
  name: string;
  title: string;
  photoSrc: string;
}>();
</script>

<style scoped>
.profile-container {
  display: flex;
  align-items: center;
  gap: 30px;
  margin-bottom: 1.5em;
}

.profile-info {
  flex: 2;
}

.profile-image {
  flex: 1;
  text-align: center;
}

.profile-photo {
  max-width: 270px;
  border-radius: 5px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  transition: transform 0.3s ease;
}

.profile-photo:hover {
  transform: scale(1.03);
}

.social-links {
  margin-top: 10px;
}

.social-link {
  color: #527bbd;
  text-decoration: none;
  font-weight: 500;
  transition: color 0.3s;
}

.social-link:hover {
  color: #2a4a8c;
  border-bottom: 1px solid;
}

@media (max-width: 768px) {
  .profile-container {
    flex-direction: column-reverse;
    text-align: center;
  }
}
</style>
