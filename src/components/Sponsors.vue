<template>
  <div class="sponsors wow animate__animated animate__backInLeft">
    <div class="coinbase">
      <div class="one-block">
        <img src="../assets/img/coinbase.png" class="one" alt="coinbase" />
        <img src="../assets/img/blockchain.png" class="two" alt="blockchain" />
      </div>
      <div class="two-block">
        <img src="../assets/img/binance.png" class="three" alt="binance" />
        <img src="../assets/img/bitmex.png" class="four" alt="bitmex" />
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.sponsors {
  display: flex;
  justify-content: center;
  margin-top: 210px;
  margin-left: 220px;
  .coinbase {
    display: flex;
    .one {
      margin-right: 132px;
    }
    .two {
      margin-right: 132px;
    }
    .three {
      margin-right: 132px;
    }
    .four {
      margin-right: 132px;
    }
  }
}

@media (max-width: 1588px) {
  .sponsors {
    margin-left: 150px;
    display: flex;
    justify-content: center;
  }
}

@media (max-width: 1518px) {
  .sponsors {
    .coinbase {
      .one {
        margin-right: 102px;
      }
      .two {
        margin-right: 102px;
      }
      .three {
        margin-right: 102px;
      }
      .four {
        margin-right: 102px;
      }
    }
  }
}

@media (max-width: 1456px) {
  .sponsors {
    margin-left: 120px;
  }
  .four {
    margin-right: 0px;
  }
}

@media (max-width: 1370px) {
  .sponsors {
    margin-left: 70px;
  }
}

@media (max-width: 1320px) {
  .sponsors {
    .coinbase {
      .one {
        margin-right: 52px;
      }
      .two {
        margin-right: 52px;
      }
      .three {
        margin-right: 52px;
      }
      .four {
        margin-right: 52px;
      }
    }
  }
}

@media (max-width: 1170px) {
  .sponsors {
    margin-left: 0px;
    .coinbase {
      display: block;
      .one-block {
        .one {
          margin-right: 150px;
        }
      }
      .two-block {
        margin-top: 52px;
        .three {
          margin-right: 150px;
        }
      }
    }
  }
}

@media (max-width: 768px) {
  .sponsors {
    .coinbase {
      .one-block {
        .one {
          margin-right: 70px;
        }
        .two {
          margin-right: 0px;
        }
      }
      .two-block {
        .three {
          margin-right: 70px;
        }
        .four {
          margin-right: 0px;
        }
      }
    }
  }
}

@media (max-width: 600px) {
  .sponsors {
    .coinbase {
      .one-block {
        .one {
          width: 120px;
        }
        .two {
          width: 260px;
        }
      }
      .two-block {
        .three {
          width: 120px;
        }
        .four {
          width: 120px;
        }
      }
    }
  }
}

@media (max-width: 500px) {
  .sponsors {
    margin-top: 100px;
    .coinbase {
      .one-block {
        .two {
          width: 200px;
        }
      }
    }
  }
}
</style>
