<template>
  <q-page class="column justify-center items-center">
    <div class="row items-center justify-around container-logo q-mt-xl">
      <q-img src="../assets/logo-white.png" width="55px" />
      <strong>Daniel</strong>
    </div>
    <q-icon
      name="keyboard_arrow_down"
      class="q-icon-arrow"
      size="28px"
    ></q-icon>

    <q-card class="my-card q-ma-lg" flat bordered>
      <q-card-section horizontal class="q-pa-lg">
        <div class="container-card">
          <q-icon name="payment" size="35px" class="q-icon-card"></q-icon>
          <div class="info-container q-mt-xl">
            <strong class="text-uppercase">Fatura Atual</strong>
            <h4 class="q-ma-none">R$ 1.258,40</h4>
            <div>
              <span>Limite disponível</span>
              <strong class="q-ml-sm text-uppercase">r$ 4.830,00</strong>
            </div>
          </div>
        </div>

        <q-card-actions vertical class="column justify-center">
          <div class="div-orange"></div>
          <div class="div-blue"></div>
          <div class="div-green"></div>
        </q-card-actions>
      </q-card-section>
      <div
        class="bottom-container row items-center justify-between q-pa-sm q-mb-md q-mx-sm"
      >
        <q-icon size="25px" name="fastfood"></q-icon>
        <span class="q-mx-sm"
          >Compra mais recente em Catina Nero no valor de R$ 84,00 hoje</span
        >
        <q-icon size="20px" name="keyboard_arrow_right"></q-icon>
      </div>
    </q-card>

    <q-scroll-area horizontal class="q-ml-md q-my-md">
      <div class="row no-wrap">
        <q-card class="card-items column justify-between q-ml-sm">
          <q-card-section>
            <q-icon name="person_add" size="35px"></q-icon>
          </q-card-section>

          <q-card-section class="q-pt-none">
            <strong> Indicar amigos </strong></q-card-section
          >
        </q-card>
        <q-card class="card-items column justify-between q-ml-sm">
          <q-card-section>
            <q-icon name="monetization_on" size="35px"></q-icon>
          </q-card-section>

          <q-card-section class="q-pt-none">
            <strong> Depositar </strong></q-card-section
          >
        </q-card>
        <q-card class="card-items column justify-between q-ml-sm">
          <q-card-section>
            <q-icon name="request_quote" size="35px"></q-icon>
          </q-card-section>

          <q-card-section class="q-pt-none">
            <strong> Transferir </strong></q-card-section
          >
        </q-card>
        <q-card class="card-items column justify-between q-ml-sm">
          <q-card-section>
            <q-icon name="receipt" size="35px"></q-icon>
          </q-card-section>

          <q-card-section class="q-pt-none">
            <strong> Pagar boleto </strong></q-card-section
          >
        </q-card>
      </div>
    </q-scroll-area>
  </q-page>
</template>

<script>
export default {
  name: "PageIndex",
};
</script>


<style lang="scss" scoped>
.q-icon {
  cursor: pointer;
}
.container-logo {
  width: 40%;
  strong {
    color: #ffe8ff;
    font-size: 22px;
  }
}
.q-icon-arrow {
  color: #ffe8ff;
}
.q-icon-card {
  color: #363538;
}
.my-card {
  width: 100%;
  max-width: 330px;
  height: 340px;
}
.info-container {
  height: 100px;
  h4 {
    color: #19afba;
    font-weight: bold;
  }

  strong:first-child {
    color: #19afba;
  }
  span {
    color: #363538;
  }

  strong {
    color: #9cd130;
  }
}

.container-card {
  width: 95%;
}

.div-orange {
  height: 30px;
  width: 7px;
  background-color: #ecad21;
  border-top-right-radius: 5px;
  border-top-left-radius: 5px;
}
.div-blue {
  height: 70px;
  width: 8px;
  background-color: #19afba;
}
.div-green {
  height: 105px;
  width: 7px;
  background-color: #9cd130;
  border-bottom-right-radius: 5px;
  border-bottom-left-radius: 5px;
}

.bottom-container {
  .q-icon {
    color: #363538;
  }
  span {
    color: #363538;
    width: 75%;
  }
}

.card-items {
  height: 140px;
  width: 115px;
  background-color: #923fa9;
  color: #ffe8ff;
  cursor: pointer;
}

.q-scrollarea {
  width: 95%;
  height: 145px;
}
</style>
