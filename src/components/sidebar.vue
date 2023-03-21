<template>
  <div class="side-bar col-md-2 side-menu" id="side-menu">
    <ul v-for="(navItem, i) in navItems" :key="i">
        <li><a href="#">{{ navItem }}</a></li>
      </ul>
    </div>
    <div class="humbugger" onclick="toogle_side_menu()" id="humbugger">
		        <img src="../assets/images/icons/menu.png" alt="menu icon" @click="toogle_sidebar()">
		    </div>
</template>

<script>
export default {
  data () {
    return {
      navItems : ["About Us", "Our Team", "Calculators", "Contact Us"],
    }
  },

  methods : {
    toogle_sidebar () {
      if (document.getElementById("side-menu").style.display == "none") {
        document.getElementById("side-menu").style = "display : block; width: 200px;";

      }
      else
      {
        document.getElementById("side-menu").style.display = "none";
      }
    }
  },
}
</script>

<style>

</style>