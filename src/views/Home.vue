<template>
  <div>
    <Nav :menu="menu" @openMenu="openMenu" @closeMenu="closeMenu" />
    <Menu @menuClick="scrollTo($event)" v-show="menu" />
    <div>
      <AboutUs id="about_us" />
      <SmartContractAudit id="smart_contrants_audit" />
      <div class="container">
        <div style="padding: 10px 30px; text-align: center; max-width: 540px; margin: auto; border-left: 1px solid #0f2a63; border-right: 1px solid #0f2a63; border-radius: 50px">
          IF NO VULNERABILITIES OR ISSUES WERE FOUND AND YOUR CONTRACT IS 100 CORRECT THEN THE AUDIT IS FREE
        </div>
        <GetStarted />
        <FreeQuote style="padding-bottom: 50px" />
      </div>
    </div>
  </div>
</template>

<script>
import Nav from '@/components/Nav.vue'
import FreeQuote from '@/components/FreeQuote.vue'
import GetStarted from '@/components/GetStarted.vue'
import SmartContractAudit from '@/components/SmartContractAudit.vue'
import AboutUs from '@/components/AboutUs.vue'
import Menu from '@/components/Menu.vue'

export default {
  name: 'Home',
  components: {
    Nav,
    FreeQuote,
    GetStarted,
    SmartContractAudit,
    AboutUs,
    Menu
  },
  data () {
    return {
      menu: false
    }
  },
  methods: {
    openMenu () {
      this.menu = true
    },
    closeMenu () {
      this.menu = false
    },
    scrollTo (id) {
      this.closeMenu()
      const element = document.getElementById(id)
      element.scrollIntoView({ behavior: 'smooth' })
    }
  }
}
</script>
