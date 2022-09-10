<template>
  <div class="container">
    <h1 class="task-title">Next task title</h1>
    <div class="wrapper">
      <h2 class="due">Next task due date</h2>
      <div class="button-wrapper">
        <button class="red-button">Remove task</button>
        <button class="green-button">Set as current</button>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  width: calc(100% - 2rem);
  height: calc(100% -2rem);

  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 2rem;

  min-height: 10rem;
  padding: 1rem;
  background-color: var(--gray);
  border-radius: 10px;
}
.task-title {
  border-bottom: solid 3px var(--green);
}
</style>
