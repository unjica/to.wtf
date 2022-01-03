<template>
  <div>
    <div class="mobile" style="display: flex; flex-direction: column; align-items: flex-end">
      <span style="margin: 0 20px">ABOUT US</span>
      <div class=hr></div>
    </div>
    <div class="desktop" style="height: 30px"></div>
    <div class="desktop" style="position: absolute; width: 100%; transform: translateY(100px)">
      <div class="container">
        <h4 style="width: 110px !important; direction: rtl">ABOUT US</h4>
      </div>
      <div class="hr desktop" style="z-index: 0;"></div>
    </div>
    <div class="container" style="padding-top: 20px; margin: 0 auto">
      <div style="position: relative;">
        <div style="display: flex; align-items: flex-end;">
          <h1 class="mobile" style="padding: 20px">BLOCKCHAIN ANS SMART CONTRACTS SOFTWARE DEVELOPMENT</h1>
          <div class="desktop" style="margin-left: 110px; ">
            <h1 style="padding-left: 20px;">BLOCKCHAIN ANS SMART</h1>
            <h1 style="padding-left: 20px;">CONTRACTS SOFTWARE</h1>
            <h1 style="padding: 0 50px 0 20px; position: relative; width: fit-content; background-color: #d9dbda; z-index: 1">DEVELOPMENT</h1>
          </div>
        </div>
      </div>
    </div>
    <!-- <div style="position: absolute; right: 0; left: 0">
      <div class="container">
        <h4 style="width: 110px !important; direction: rtl">ABOUT US</h4>
      </div>
      <div class="hr desktop" style="z-index: 0;"></div>
    </div> -->
    <div class="container">
      <p class="alpina desktop" style="font-size: 20px; margin: 10px 0 10px 130px; max-width: 540px">
        We utilize our expertise and passion to build blockchain based solutions to empower businesses and inventive entrepreneurs to automate operations, integrate and upgrade novel and legacy systems, or build from conception to delivery that drive  measurable results.
      </p>
      <p class="alpina mobile" style="font-size: 20px; margin: 0 20px;">
        We utilize our expertise and passion to build blockchain based solutions to empower businesses and inventive entrepreneurs to automate operations, integrate and upgrade novel and legacy systems, or build from conception to delivery that drive  measurable results.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AboutUs'
}
</script>
