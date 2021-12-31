<template>
  <div>
    <Nav />
    <div class="hr" style="position: absolute; z-index: 0; transform: translateY(150px)"></div>
    <div class="container" style="padding-top: 50px">
      <div style="position: relative">
        <div style="display: flex; align-items: flex-end;">
          <span style="margin: 0 0 20px 0; width: 110px; text-align: end">ABOUT US</span>
          <div>
            <h1 style="padding-left: 20px;">BLOCKCHAIN ANS SMART </h1>
            <h1 style="padding-left: 20px;">CONTRACTS SOFTWARE</h1>
            <h1 style="padding: 0 50px 0 20px; position: relative; width: fit-content; background-color: #d9dbda; z-index: 1">DEVELOPMENT</h1>
          </div>
        </div>
      </div>
      <p class="alpina" style="font-size: 20px; margin: 10px 0 10px 130px; max-width: 540px">
        We utilize our expertise and passion to build blockchain based solutions to empower businesses and inventive entrepreneurs to automate operations, integrate and upgrade novel and legacy systems, or build from conception to delivery that drive  measurable results.
      </p>
      <div style="border-radius: 50%; padding: 40px 10px; font-size: 20px; border: solid 1px #0f2a63; display: flex; justify-content: center; align-items: center; margin: 100px auto 0; max-width: 440px; text-align: center">
        Let's build the smart contracts you need!
      </div>
      <div style="margin: auto; width: fit-content; height: 40px; width: 1px; background-color: #0f2a63"></div>
      <div style="margin: auto; width: 20px; height: 20px; border-bottom: 1px solid #0f2a63; border-right: 1px solid #0f2a63; transform: rotate(45deg) translate(-17px, -16.7px)"></div>
    </div>
    <div class="hr" style="position: absolute; z-index: 0; transform: translateY(210px)"></div>
    <div class="container">
      <div style="margin-top: 100px">
        <div class="container" style="padding-top: 50px; margin-bottom: 50px">
          <div style="position: relative">
            <div style="display: flex; align-items: flex-end;">
              <span style="margin: 0 0 20px 0; width: 110px; text-align: end">
                <div>SMART</div>
                <div>CONTRACT</div>
                <div>AUDIT</div>
              </span>
              <div>
                <h1 style="padding-left: 20px;">WE PROVIDE THE</h1>
                <h1 style="padding: 0 50px 0 20px; position: relative; width: fit-content; background-color: #d9dbda; z-index: 1">FOLLOWING SERVICES</h1>
              </div>
            </div>
          </div>
          <ul class="alpina" style="list-style-type: none; font-size: 20px; margin: 10px 0 10px 130px; max-width: 540px">
            <li>Check against the latest attack vectors and give you a full pdf audit report.</li>
            <li>Check against any logical errors.</li>
            <li>We leverage a combination of static analysis, automated tools, and a robust manual review process to provide industry-leading security recommendations to project teams.</li>
            <li>We assist project team's in resolve any outstanding issues or implementing our recommendations.</li>
          </ul>
          <div style="height: 10px"></div>
          <div style="margin: auto; display: flex; max-width: 540px; align-items: flex-start;">
            <div style="margin-right: 25px; background-color: #fff; border: 1px solid #000; border-radius: 50%; width: 30%; padding: 20px 0; display: flex; justify-content: center; align-items: center">NOTE THAT</div>
            <ul style="width: 70%; margin-top: 20px">
              <li>Normal price per audit $1000-$5000, time to deliver 1-3 days</li>
              <li>100% Refund if we don't meet the deadline</li>
              <li>The audit is confidental. It's up to you to do whatever you want with it after</li>
              <li>We can only audit smart contracts that are on etherum, binance smart chain (bsc), polygon (matic), fantom, avalance's c-chain, harmony one, kucoin (kcc), huobi eco, arbitrum, or any other evm-compatible side-chain or 12 chain</li>
            </ul>
          </div>
        </div>
        <div style="padding: 10px 30px; max-width: 540px; margin: auto; border-left: 1px solid #0f2a63; border-right: 1px solid #0f2a63; border-radius: 50px">
          IF NO VULNERABILITIES OR ISSUES WERE FOUND AND YOUR CONTRACT IS 100 CORRECT THEN THE AUDIT IS FREE
        </div>
        <div style="max-width: 540px; margin: 50px auto;">
          <h2 style="margin-bottom: 10px">HOW TO GET STARTED:</h2>
          <ul style="margin-left: 20px">
            <li>link to the deployed smart contract on the testnet/mainnet</li>
            <li>or link to github repo</li>
            <li>or the contracts zipped</li>
            <li>additionally if you have tests written it will greatly improve the audit delivery time</li>
          </ul>
        </div>
        <div style="padding: 0 0 50px">
          <div style="background-color: #B3E6BE; border-radius: 10px; text-align: center; margin: auto; width: fit-content; padding: 20px; border: 1px solid #000">
            <p style="margin-bottom: 10px">GET A FRREE QUOTE</p>
            <div>
              <img width="30" style="margin: 0 10px;" src="../assets/send.png" alt="send">
              <img width="30" style="margin: 0 10px;" src="../assets/message.png" alt="message">
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Nav from '@/components/Nav.vue'

export default {
  name: 'Home',
  components: {
    Nav
  }
}
</script>
