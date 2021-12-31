<template>
  <div style="background-color: #B3E6BE; position: fixed; top: 0; left: 0; right: 0; bottom: 0; z-index: 2; display: flex; flex-direction: column; justify-content: center; align-items: center;">
    <ul style="font-size: 30px">
      <li class="pointer" @click="$emit('menuClick', 'about_us')">ABOUT US</li>
      <li class="pointer" @click="$emit('menuClick', 'smart_contrants_audit')">SMART CONTRACTS AUDIT</li>
      <li>CRYPTO ASSETS RECOVERY</li>
      <li>BLOCKCHAIN FORENSICS</li>
      <li>NFT PROJECTS</li>
      <li>TOKENOMICS</li>
      <li>DAO</li>
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
</style>
