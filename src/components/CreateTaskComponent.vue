<template>
  <div class="container">
    <input class="text-input" type="text" placeholder="Add new task..." />
    <div class="additional-options">
      <button class="create-button">Create</button>
    </div>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  background-color: var(--gray);
  padding: 1rem;
  border-radius: 10px;
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
.create-button {
  background-color: transparent;
  border: solid 2px var(--green);
  border-radius: 5px;
  padding: 0.5rem;
  font-size: 1.2rem;
  color: white;
  font-weight: 500;
  letter-spacing: 0.05rem;
}
.additional-options{
    display: flex;
    padding: 1rem 0;
}
.create-button:hover {
  background-color: var(--green);
  color: var(--dark);
}
</style>
