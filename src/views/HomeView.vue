<script>
import CreateTask from "../components/CreateTaskComponent.vue";
import ClockComponent from "../components/ClockComponent.vue";
export default { components: { CreateTask, ClockComponent } };
</script>

<template>
  <div class="home-container">
    <div id="create-task">
      <CreateTask></CreateTask>
    </div>
    <div id="clock">
      <ClockComponent></ClockComponent>
    </div>
    <div id="current-task"></div>
    <div id="next-task"></div>
    <div id="task-list"></div>
  </div>
</template>

<style>
.home-container {
  width: 100%;
  height: 100vh;
  display: grid;
  grid-template-areas:
    "clock current-task task-list"
    "clock current-task task-list"
    "create-task next-task task-list";
}
#create-task {
  grid-area: create-task;
}
#clock {
  grid-area: clock;
}
#current-task {
  grid-area: current-task;
}
#next-task {
  grid-area: next-task;
}
#task-list {
  grid-area: task-list;
}
</style>
