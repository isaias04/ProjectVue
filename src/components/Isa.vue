<template>
    <div class="Isa"></div>
    <h2>Menu</h2>
    <ul>
        <li>
            <Router-link to="/ListadoTareas">lista de tareas</Router-link>
        </li>
        <li> <Router-link to="/contador">contador</Router-link>
        </li>
       
    </ul>
</template>
<script setup></script>

<style scoped>
.Isa {
    width: 200px;
    color: rgb(151, 149, 149);
    padding: 20px;
}
</style>
