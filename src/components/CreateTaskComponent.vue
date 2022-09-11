<template>
  <div class="container">
    <input class="text-input" type="text" placeholder="Add new task..." />
    <div class="additional-options">
      <button class="green-button" @click="creating= !creating">Create</button>
    </div>
  </div>
  <CreateFormComponent
    v-if="creating"
    :creating="creating"
  ></CreateFormComponent>
</template>

<script>
import CreateFormComponent from "./CreateFormComponent.vue";

export default {
  data: function () {
    return {
      creating: false,
    };
  },
  components: {
    CreateFormComponent,
  },
};
</script>

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
.additional-options {
  display: flex;
  flex-direction: row-reverse;
  padding: 1rem 0;
}
</style>
