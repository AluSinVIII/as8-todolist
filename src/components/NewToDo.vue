<!-- ./component/NewToDo.vue -->
<script>

export default {
    name: "NewToDo"
}
</script>

<template>
<div id = "NewToDo" class="control">
  <input v-model="task" type="text" placeholder="Ajouter une tâche ..."><br><br>
  <button @click="savetask" class="button is-primary"><i class="fas fa-plus-circle"></i></button>


</div>
</template>
<style>
#NewToDo{
    display: flex;
    align-items: center;
    justify-content: center;

    
}
</style>