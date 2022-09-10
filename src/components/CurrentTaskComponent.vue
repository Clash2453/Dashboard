<template>
  <div class="container">
    <h1 class="task-title">Current task</h1>
    <p class="task-description">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque
      perferendis culpa exercitationem, placeat possimus cumque. Nemo saepe
      natus doloribus nisi quae nam, quidem cumque voluptatum beatae molestiae
      fuga, atque aliquid.
    </p>
    <div class="wrapper">
      <h2 class="due">Due time</h2>
      <div class="button-wrapper">
        <button class="red-button">Discard</button>
        <button class="green-button">Mark done</button>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: var(--gray);
  width: calc(100% - 2rem);
  height: fit-content;
  border-radius: 10px;
  padding: 1rem;
  gap: 2rem;
}
.task-description {
  width: calc(100% - 2rem);
  height: fit-content;
  max-height: 20rem;
  font-family: "Lato", sans-serif;
  color: whitesmoke;
  background-color: rgba(255, 255, 255, 0.1);
  border-radius: 5px;
  font-size: 1.3rem;
  line-height: 1.5rem;
  padding: 1rem;
  overflow: auto;
}
</style>
