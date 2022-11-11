<template>
  <div class="col-md-12">
    <ul>
      <li><a href="">Home</a></li>
      <li><a href="">Projectos</a></li>
      <li><a href="">Contacto</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
div {
  background-color: #ccc;
}

ul {
  list-style: none;
  display: flex;
}

li {
  margin-right: 10px;
}

a {
  color: #ddd;
  text-decoration: none;
  transition: 0.5s;
}

a:hover {
  color: turquoise;
}
</style>