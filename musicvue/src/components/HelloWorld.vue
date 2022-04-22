<template>
  <div class="hello">
    <p></p>
    <h3>{{ msg }}</h3>
    <br>
    <p>
      Bienvenidos a nuestro  proyecto como presentación<br>
      de nuestro parcial para la asignatura Programación <br>
      computacional IV. Si quieren visitar el repositorio de <br>
      el proyecto, pueden acceder a este
      <a href="https://github.com/KatyaViscarra/Parcial-II.git" target="_blank" rel="noopener">link</a>.
    </p>
    <h5>Breve Introducción</h5>
    <ul>
    <p>
      En este sitio web se presentará la conexión "exitosa" de <br>
      nuestra API creada en el entorno Laravel, mostrando los <br>
      datos de nuestra base de datos en formato de una tabla, <br>
      categorizando la información mediante el id, seguido por <br>
      el nombre, tipo, descripción y género.
    </p>
    <br>
    <p>Nuestro enfoque está relacionado a la música y el teatro <br>
    debido a que ese fue la tematica asignada.

    </p>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
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
