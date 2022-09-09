<script>
export default {
  data: function () {
    return {};
  },
};
</script>

<template>
  <nav class="nav-bar">
    <ul class="nav-list">
      <router-link to="/" class="nav-link">Home</router-link>
      <router-link to="/calendar" class="nav-link">Calendar</router-link>
      <router-link to="/inbox" class="nav-link">Inbox</router-link>
    </ul>
  </nav>

  <router-view></router-view>
</template>

<style scoped>
.nav-bar {
  width: calc(100% - 2rem);
  height: fit-content;
  padding: 1rem;
  background: rgb(34, 34, 34);
  padding: 0.5rem 1rem;
}
.nav-list {
  display: flex;
  flex-direction: row-reverse;
}
</style>
