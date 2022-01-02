<template>
  <div>
    <Nav :menu="menu" @openMenu="openMenu" @closeMenu="closeMenu" />
    <Menu @menuClick="scrollTo($event)" v-show="menu" />
    <div class="mobile" style="height: 80px"></div>
    <div>
      <AboutUs id="about_us" />
      <div class="margin" style="border-radius: 50%; padding: 40px 10px; font-size: 20px; border: solid 1px #0f2a63; display: flex; justify-content: center; align-items: center; margin-top: 50px !important; max-width: 440px; text-align: center">
        Let's build the smart contracts you need!
      </div>
      <div style="margin: auto; width: fit-content; transform: translateY(-0.5px)">
        <img style="transform: rotate(90deg); width: 30px; margin: 0 auto" src="@/assets/arrow.png" alt="arrow">
      </div>
      <div style="height: 100px"></div>
      <SmartContractAudit id="smart_contrants_audit" />
      <CryptoAssetsRecovery id="crypto_assets_recovery" />
      <BlockchainForensics id="blockchain_forensics" />
      <NftProjects id="nft_projects" />
      <Tokenomics id="tokenomics" />
      <Dao id="dao" />
      <div class="container">
        <div class="margin" style="padding: 10px 30px; text-align: center; max-width: 540px; border-left: 1px solid #0f2a63; border-right: 1px solid #0f2a63; border-radius: 50px">
          IF NO VULNERABILITIES OR ISSUES WERE FOUND AND YOUR CONTRACT IS 100 CORRECT THEN THE AUDIT IS FREE
        </div>
        <GetStarted class="margin" />
        <FreeQuote style="padding-bottom: 50px" />
      </div>
    </div>
  </div>
</template>

<script>
import Nav from '@/components/Nav.vue'
import FreeQuote from '@/components/FreeQuote.vue'
import GetStarted from '@/components/GetStarted.vue'
import SmartContractAudit from '@/components/sections/SmartContractAudit.vue'
import AboutUs from '@/components/sections/AboutUs.vue'
import Menu from '@/components/Menu.vue'
import CryptoAssetsRecovery from '@/components/sections/CryptoAssetsRecovery.vue'
import BlockchainForensics from '@/components/sections/BlockchainForensics.vue'
import NftProjects from '@/components/sections/NftProjects.vue'
import Tokenomics from '@/components/sections/Tokenomics.vue'
import Dao from '@/components/sections/Dao.vue'

export default {
  name: 'Home',
  components: {
    Nav,
    FreeQuote,
    GetStarted,
    SmartContractAudit,
    AboutUs,
    Menu,
    CryptoAssetsRecovery,
    BlockchainForensics,
    NftProjects,
    Tokenomics,
    Dao
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
