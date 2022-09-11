<template>
  <div class="form-container">
    <h1></h1>
    <label class="input-container" for="">
      Title
      <input class="text-input" type="text" name="" id="title" />
    </label>
    <label class="input-container" for="">
      Description
      <input class="text-input" type="text" name="" id="description" />
    </label>
    <label class="input-container" for="">
      Deadline:<br />
      <input
        class="text-input"
        :value="dueDate"
        type="datetime-local"
        name=""
        id="due-date"
      />
    </label>
    <div class="button-wrapper">
      <button class="red-button">Discard</button>
      <button class="green-button">Create</button>
    </div>
  </div>
</template>

<script>
export default {
  props: ["creating"],
  data: function () {
    return {
      dueDate: "",
    };
  },
};
</script>

<style scoped>
.form-container {
  position: fixed;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  background-color: var(--gray);

  width: 20rem;
  height: 25rem;

  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

  gap: 1rem;

  border-radius: 10px;
}
.input-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
}
</style>
