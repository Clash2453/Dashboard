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
      <router-link to="/calendar" class="nav-link">Calendar</router-link>
      <router-link to="/inbox" class="nav-link">Inbox</router-link>
      <router-link to="/" class="nav-link">Home</router-link>
    </ul>
  </nav>
  <div class="container">
    <router-view></router-view>
  </div>
</template>

<style scoped>
.nav-bar {
  width: calc(100% - 2rem);
  height: fit-content;
  padding: 1.5rem;
  background: hsl(0, 0%, 12%);
  padding: 0.5rem 1rem;
  border-bottom: solid 3px var(--green);
}
.nav-list {
  display: flex;
  flex-direction: row-reverse;
}
.container {
  padding: 1rem;
}
</style>
