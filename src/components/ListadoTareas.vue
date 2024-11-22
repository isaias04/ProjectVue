<template>
    <div>
        <h2>listado de tareas </h2>
        <input type="text" v-model="NuevaTarea" @keyup.enter="addTarea">
        <ul>
            <li  v-for="(tarea, index) in tareas" :key="index">
                {{ tarea }}
                <button class="estilo" @click="BorrarTarea">Borrar</button>
            </li>

        </ul>
    </div>
</template>
<script setup>
import { ref } from 'vue';
const tareas = ref ([]);
const NuevaTarea = ref('');
const addTarea =() => {
    tareas.value.push(NuevaTarea.value);
    NuevaTarea.value = '';
}
const BorrarTarea =(index) => {
    tareas.value.splice(index,1);
}
</script>
<style scoped>
.estilo {
    padding: 10px 20px;
    background-color: #ff0202;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}
</style>