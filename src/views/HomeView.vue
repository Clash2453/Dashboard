<script>
import CreateTask from "../components/CreateTaskComponent.vue";
import ClockComponent from "../components/ClockComponent.vue";
import CurrentTaskComponent from "../components/CurrentTaskComponent.vue";
import NextTaskComponent from "../components/NextTaskComponent.vue";
import TaskListComponent from "../components/TaskListComponent.vue";
export default {
  components: {
    CreateTask,
    ClockComponent,
    CurrentTaskComponent,
    NextTaskComponent,
    TaskListComponent,
  },
};
</script>

<template>
  <div class="home-container">
    <div class="component-container" id="create-task">
      <CreateTask></CreateTask>
    </div>
    <div class="component-container" id="clock">
      <ClockComponent></ClockComponent>
    </div>
    <div class="component-container" id="current-task">
      <CurrentTaskComponent></CurrentTaskComponent>
    </div>
    <div class="component-container" id="next-task">
      <NextTaskComponent></NextTaskComponent>
    </div>
    <div class="component-container" id="task-list">
      <TaskListComponent></TaskListComponent>
    </div>
  </div>
</template>

<style>
.home-container {
  width: 100%;
  height: calc(100vh - (60px + 2rem));
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr;
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
