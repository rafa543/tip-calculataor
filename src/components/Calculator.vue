<template>
  <v-container>
    <v-row class="d-flex justify-center">
      <div class="calculator d-flex justify-space-between">

        <div class="form">

          <div class="bill">
            <span>Bill</span>
            <div class="Appetizer mt-2">
                <v-text-field
                class="centered-input text--darken-3 mt-3" 
                dense
                outlined
                prepend-inner-icon="mdi-currency-usd"
              ></v-text-field>

          </div>

          <div class="percent mb-8">
            <span>Select Tip %</span>

            <div class="tip mt-4">
              <v-col cols="12" md="12" class="d-flex justify-space-between pa-0">
                <v-btn
                  class="btn-tip"
                  elevation="1"
                  large
                >5%</v-btn>
                <v-btn
                  class="btn-tip"
                  elevation="1"
                  large
                >10%</v-btn>
                <v-btn
                  class="btn-tip"
                  elevation="1"
                  large
                >15%</v-btn>

              </v-col>
            </div>

            <div class="tip mt-4">
              <v-col cols="12" md="12" class="d-flex justify-space-between pa-0">
                <v-btn
                  class="btn-tip"
                  elevation="1"
                  large
                >25%</v-btn>
                <v-btn
                  class="btn-tip"
                  elevation="1"
                  large
                >50%</v-btn>
                <v-btn
                  class="btn-tip"
                  elevation="1"
                  large
                >Custom</v-btn>

              </v-col>
            </div>
          </div>

          <div class="percent">
            <span>Number of People</span>

            <v-text-field
                class="mt-2"
                dense
                outlined
                prepend-inner-icon="mdi-account"
              ></v-text-field>
          </div>

        </div>

        
        </div>

        <div class="results-tip d-flex-column align-center">
          <v-row>
            <v-col
                cols="6"
                sm="6"
                >
            <p>Tip Amount</p>
            <span>/ person</span>
            </v-col>

            <v-col
              cols="6"
                sm="6"
                >
              <h2>$4.27</h2>
            </v-col>

          </v-row>

          <v-row>
            <v-col
                cols="6"
                sm="6"
                >
            <p>Total</p>
            <span>/ person</span>
            </v-col>

            <v-col
              cols="6"
                sm="6"
                >
              <h2>$32.79</h2>
            </v-col>



          </v-row>

          <v-row>
            <v-col cols="6"
                sm="6">
              <v-btn
              
              class="btn-reset"
              elevation="2"
            >Reset</v-btn>
            </v-col>
          </v-row>
        </div>
      </div>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'Calculator',

  }
</script>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&display=swap');

  .calculator {
    width: 800px;
    padding: 30px 30px 30px 30px;
    background: hsl(0, 0%, 100%);
    border-radius: 20px;
  }
  .v-text-field>>> input {
    text-align: end;
    font-family: 'Space Mono', monospace;
    font-size: 25px;
    font-weight: bold;
  }

  span {
    font-family: 'Space Mono', monospace;
    color: hsl(183, 100%, 15%);
    font-weight: 700;
  }
  .form {
    width: 350px;
  }
  .v-btn:not(.v-btn--round).v-size--large{
    min-width: 105px;
    background: hsl(183, 100%, 15%);
    color: white;
    font-family: 'Space Mono', monospace;
    font-size: 17px;
  }

  .results-tip {
    background: hsl(183, 100%, 15%);
    font-family: 'Space Mono', monospace;
    width:350px;
    border-radius: 20px;
  }

  .results-tip p{
    margin-top: 40px;
    margin-left: 40px;
    margin-bottom: -2px;
    color: white;
  }

  .results-tip span {
    margin-left: 40px;
    font-size: 14px;
    color: hsl(184, 14%, 56%);
  }

  .results-tip h2{
    font-family: 'Space Mono', monospace;
    color:hsl(172, 67%, 45%);
    text-align: end;
    font-size: 35px;
    margin-top: 35px;
    margin-right: 20px;
  }

  .btn-reset {
    width: 300px;
    height: 45px !important;
    margin: 80px 20px 0 25px;
    background:hsl(172, 67%, 45%) !important;
    font-weight: bold;
  }


</style>
