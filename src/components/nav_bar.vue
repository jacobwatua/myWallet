<template>
  <div class="NavBar">
    <ul v-for="(navItem, i) in navItems" :key="i">
      <li><a href="#">{{ navItem }}</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  data () {
    return {
      navItems : ["About Us", "Our Team", "Calculators", "Contact Us"],
    }
  },
}
</script>

<style>
  .NavBar{
    background-color: #1B1B1B;
    box-shadow: 0px 1px 3px rgba(255, 255, 255, 0.1);
    height: 70px;
    box-sizing: border-box;
    padding-top: 15px;
    color: white;
    position: fixed;
    top: 0px;
    width: 100%;
    z-index: 99;
  }
  .NavBar ul{
    list-style: none;
    display: inline-flex;
    margin-left: 100px;
  }
  .NavBar ul li{
    margin-left: 40px;
    margin-right: 10px;
    padding: 8px;
  }
  .NavBar ul li a {
    text-decoration: none;
    color: white;
  }
</style>