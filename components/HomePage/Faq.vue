<template>
  <v-card elevation="0" class="faq">
    <h1 class="faq-title">Frequently Asked Questions</h1>
    <div>
      <div>
        <v-tabs class="tabs" v-model="tab">
          <v-tabs-slider color="#FF6600"></v-tabs-slider>

          <v-tab v-for="item in items" :key="item" class="faq-tabs">
            {{ item }}
          </v-tab>
        </v-tabs>
      </div>
    </div>

    <v-tabs-items v-model="tab">
      <v-tab-item v-for="item in items" :key="item" class="faq-item">
        <v-card elevation="0" flat>
          <v-card-text class="faq-section d-flex align-items-center">
            <div class="number">1</div>
            <div class="mt-1">
              <p class="faq-question text text-left font-weight-bold">
                How can company best begin its AI journey?
              </p>
              <p class="text mb-0">
                Unstructured data is a roadblock to AI, which needs to
                standardize to capitalize on its potential.
              </p>
            </div>
          </v-card-text>
          <v-card-text class="faq-section d-flex align-items-center">
            <div class="number">2</div>
            <div class="mt-1">
              <p class="faq-question text text-left font-weight-bold">
                What are the strategic benefits of AI in tax?
              </p>
              <p class="text mb-0">
                AI will increase performance, accuracy and ROI
              </p>
            </div>
          </v-card-text>
          <v-card-text class="faq-section d-flex align-items-center">
            <div class="number">3</div>
            <div class="mt-1">
              <p class="faq-question text text-left font-weight-bold">
                How can company best begin its AI journey?
              </p>
              <p class="text mb-0">
                Tax Advisors can streamline data processes ready for AI.
              </p>
            </div>
          </v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-card>
</template>

<script>
export default {
  data() {
    return {
      tab: null,
      items: ["General", "AI Tax", "MFExcise", "Tax Advisors"],
      text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
    };
  },
};
</script>

<style lang="scss" scoped>
.faq {
  text-align: center;
  padding-bottom: 90px;

  .faq-title {
    font-family: Roboto;
    font-style: normal;
    line-height: 35px;
    font-weight: bold;
    color: #ff6600;
    margin-top: 27px;
    margin-bottom: 27px;
  }

  .v-toolbar__content {
    // height: 0 !important;
    // margin: 0 !important;
    display: none;
  }

  .tabs {
    margin-bottom: 26px;
  }

  .faq-tabs {
    width: 100%;
    margin-left: 0;
    padding-left: 0;
    font-weight: bold;
  }

  .v-tab {
    background: #dadada;
  }

  .v-tab--active {
    background: #ff6600;
    color: #ffffff;
  }

  .number {
    width: 30px;
    height: 30px;
    background: #ff6600;
    color: white;
    font-size: 16px;
    text-align: center;
    padding: auto 0;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 50%;
    margin-right: 10px;
  }

  .faq-section {
    margin-bottom: 15px;
    padding-top: 0;
    padding-bottom: 0;
    padding-left: 34px;
  }
  .faq-question {
    margin-bottom: 10px;
  }
}
</style>
