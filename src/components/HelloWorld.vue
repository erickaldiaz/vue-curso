<template>
  <div class="hello">
  <h1>el mensaje es: {{ msg }}</h1>
  <h1 v-text="msg">hola</h1>

<!-- a partir de aca V-HTML -->
  <p>esto es una etiqueta p</p>
  <p v-html="htmlEjemplo"></p>

  <!-- A PARTIR DE ACA V SHOW -->
  <h2 v-show="acceso">Tenemos accesos aa esto</h2>

  <!-- A PARTIR DE ACA v-IF -->
  <h3 v-if="accesoComun"> Tenemos acceso</h3>
  <h3 v-else-if="accesoAdministrador"> Tenemos acceso de administrador</h3>
  <h3 v-else>No tienes accesos para ver esto</h3>

  <!-- A PARTIR DE ACA v-for -->
  <div v-for="(alumno, index) in alumnos" :key="index">
    <p>{{alumno.nombre}}</p>
    <p>{{alumno.edad}}</p>
  </div>
  
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data: () => ({
    msg:'hola, bienvenidos',
    htmlEjemplo: '<p>esto es una etiqueta p</p>',
    accesoComun: false,
    accesoAdministrador: false,
    alumnos: [   
    { 
      nombre:"Matias",
      edad: 18
    },
    { 
      nombre:"Lara",
      edad: 20
    },
    { 
      nombre:"Juan",
      edad: 38
    },
    { 
      nombre:"Daina",
      edad: 25
    }
    ]
    })
  }
</script>