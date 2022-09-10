<template>
  <div class="container">
    <input class="text-input" type="text" placeholder="Add new task..." />
    <div class="additional-options">
      <button class="green-button">Create</button>
    </div>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  background-color: var(--gray);
  padding: 1rem;
  border-radius: 10px;
  width: calc(90% - 2rem);
  min-height: 10rem;
  gap: 2rem;
}
.additional-options {
  display: flex;
  width: 100%;
  flex-wrap: wrap;
}
.text-input {
  font-size: 1.5rem;
  font-family: "Lato", sans-serif;
  border: none;
  border-bottom: 3px solid var(--green);
  background-color: transparent;
  color: whitesmoke;
}

.additional-options {
  display: flex;
  flex-direction: row-reverse;
  padding: 1rem 0;
}
</style>
