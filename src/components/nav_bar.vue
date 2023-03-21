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
</style>