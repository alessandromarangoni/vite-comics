<script>
export default {
  name: "AppHeader",
}
</script>


<template>
  <div class="header_container">
    <div class="container">
      <div class="row pt-1">
        <div class="col-5 p-2 ">
          <div>
            <img src="../assets/dc-logo.png" alt="logo" class="logo">
          </div>
        </div>
        <div class="col-7 p-2 d-flex align-items-center ">
          <ul class="text-uppercase d-flex flex-wrap">
            <li><a href=""> charachters </a> </li>
            <li><a href=""> comics </a> </li>
            <li><a href=""> movies </a> </li>
            <li><a href=""> tv </a> </li>
            <li><a href=""> games </a> </li>
            <li><a href=""> collectibles </a> </li>
            <li><a href=""> videos </a> </li>
            <li><a href=""> fans </a> </li>
            <li><a href=""> news </a> </li>
            <li><a href=""> shop </a> </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.logo {
  width: 70px;
}

.header_container {
  height: 120px;
  display: flex;
}

ul li {
  display: flex;
  list-style: none;
  padding-left: 1rem;
  font-size: small;
  padding-top: 1rem;

}

ul li a {
  color: black;
  display: block;
  text-decoration: none;
}

ul li a:hover {
  border-bottom: 5px solid rgb(0, 119, 255);
}
</style>