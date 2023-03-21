<template>
    <div class="NavBar nav2" style="display : none;">
      <ul v-for="(navItem, i) in navItems" :key="i">
        <li><a href="#">{{ navItem }}</a></li>
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
}
</script>

<style>
</style>