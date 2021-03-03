<!-- ./component/ToDoCard.vue -->

<script type="text/javascript">
import NewToDo from './NewToDo.vue';
export default {
    name: "ToDoCard",
    data() {

        return {
            day: [" ","Lundi", "Mardi", "Mercredi", "Jeudi", "Vendredi", "Samedi", "Dimanche"],
            month: ["Janvier", "Février", "Mars", "Avril", "Mai", "Juin", "Juillet", "Août", "Septembre", "Octobre", "Novembre", "Décembre"],
        }

    },
    computed: {

        date: function() {
            let today = new Date();
            let todate = `${this.day[(today.getDay())]}` + ' ' + today.getDate() + ' ' + `${this.month[(today.getMonth())]}`; 
            return todate; 
        }

    },
    components: {
        NewToDo
    }
}
</script>

<template>
<div id="ToDoCard">

<div id="headTDC">
            <p>{{date}}</p>
            <p id="title">VueJs To Do List</p>
            <p> {{taskNumber}} tâches</p>
</div>
<NewToDo></NewToDo>

</div>
    
</template>
<style>
#ToDoCard{
    background-color: aliceblue;
    height: 500px;
    width: 800px;
    margin: auto ;
    border-radius: 20px;
    padding: 50px;
}

#headTDC{
    display: flex;
    justify-content: space-between;
    font-weight: bold;
}

#title{
    color: #64e7c6;
}
</style>