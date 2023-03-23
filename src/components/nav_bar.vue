<template>
    <div class="NavBar">
      <ul v-for="(navItem, i) in navItems" :key="i">
        <li @mouseover="hover_nav()"><a href="#">{{ navItem }}</a></li>
      </ul>
    </div>
    <div class="nav2">
      <div><p class="text-center"><span id="logo1">My</span><span>Wallet</span><span id="blob"></span></p></div>
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
    hover_nav () {
      document.getElementsByTagName("li")[1].style.color = "blue";
    }
  }
}
</script>

<style>
</style>