<template>
  <div class="slide-in" style="background-color: #B3E6BE; position: fixed; top: 0; left: 0; right: 0; bottom: 0; z-index: 2; display: flex; flex-direction: column; justify-content: center; align-items: center;">
    <ul style="font-size: 30px; margin: 0 0 0 20px">
      <li class="pointer" @click="$emit('menuClick', 'about_us')">ABOUT US</li>
      <li class="pointer" @click="$emit('menuClick', 'smart_contrants_audit')">SMART CONTRACTS AUDIT</li>
      <li class="pointer" @click="$emit('menuClick', 'crypto_assets_recovery')">CRYPTO ASSETS RECOVERY</li>
      <li class="pointer" @click="$emit('menuClick', 'blockchain_forensics')">BLOCKCHAIN FORENSICS</li>
      <li class="pointer" @click="$emit('menuClick', 'nft_projects')">NFT PROJECTS</li>
      <li class="pointer" @click="$emit('menuClick', 'tokenomics')">TOKENOMICS</li>
      <li class="pointer" @click="$emit('menuClick', 'dao')">DAO</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Menu'
}
</script>

<style scoped>
.pointer {
  cursor: pointer;
  transition: 0.2s;
}
.pointer:hover {
  transform: translateX(30px) scale(1.1);
  transition: 0.2s;
}
.slide-in {
  animation: slide-in 0.2s ease-out;
}
@keyframes slide-in {
  from {
    top: -100%;
  }
  to {
    top: 0;
  }
}
</style>
