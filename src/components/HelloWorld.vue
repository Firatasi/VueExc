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


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
