<template>
  <div id="app">
        <h1> {{title}} </h1>
        <hr>
        <br>
        <input type="text" v-on:input = "Change Title">
        <p>{{description}}</p>
    </div>

</template>

<script type="text/javascript">
        new Vue({
        el : "#app",
        data : {
            title : "Merhaba vue",
            description : "Bu bir açıklamadır",
        },
        methods : {
            changeTitle : function(event) {
                this.description = event.target.value;
            }
        }

        });
    </script>



