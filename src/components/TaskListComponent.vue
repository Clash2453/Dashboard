<template>
  <div class="container">
    <h1 class="task-title">Task List</h1>
    <div class="tabs">
      <h2 class="tab">Pending</h2>
      <h2 class="tab">Completed</h2>
    </div>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 90%;
  max-height: 49rem;
  width: 90%;
  background-color: var(--gray);
  border-radius: 10px;
  overflow-y: auto;
  overflow-x: hidden;
}
.tabs {
  width: calc(100% - 2rem);
  padding: 1rem;
  padding-top: 0;
  display: flex;
  align-items: center;
  gap: 0.5rem;
}
.tab {
  width: calc(50% - 1rem);
  padding: 0.5rem;
  font-family: "Lato", sans-serif;
  text-align: center;
  font-size: 1.5rem;
  color: whitesmoke;
  background-color: rgba(255, 255, 255, 0.1);
}
.task-title {
  text-align: center;
  padding: 1rem;
}
</style>
