<template>

    <link href="https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap" rel="stylesheet">

  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/contact">Contacto</router-link> |
    <router-link to="/users">Users</router-link>
  </div>
  <router-view/>

</template>

<style lang="scss">


#nav {
  padding: 30px;
  background-color: #232e7d;
  width: 65.5vw;
  margin:0 auto;
  display: flex;
  justify-content: flex-end;
  justify-content: space-around;
  font-family: 'Roboto';
  

  a {
    font-weight: bold;
    color: #ffffff;
    text-decoration:none;
    

    &.router-link-exact-active {
      color: #a6aff6;
      text-decoration:none;
    }
  }
}
</style>
