<script lang="ts">
  import rollADie from "roll-a-die";
  let dicePosition = "left";

  function response(res: Array<number>) {
      console.log(res)
      const result: HTMLInputElement = document.getElementById("result_dice") as HTMLInputElement;
      result.value = res.reduce((a, x) => {return a + x;}, 0).toString();

      const fumble = res.reduce((a, x) => {
        if (x === 1) {
          a.push(x);
        }
        return a;
      }, []);

      const critical = res.reduce((a, x) => {
        if (x === 6) {
          a.push(x);
        }
        return a;
      }, []);

      const resultMessageRollDice: HTMLDivElement = document.getElementById("result_message_roll_dice") as HTMLDivElement;
      resultMessageRollDice.innerHTML = "";

      if (critical.length >= 2) {
        resultMessageRollDice.innerHTML = "クリティカル!!";
        return;
      }

      if (fumble.length >= 2) {
        resultMessageRollDice.innerHTML = "Oops! ファンブル!";
        return;
      }
    }

  function rollDice() {
    const field: HTMLElement = document.getElementById("field_roll_dice");
    const inputNumberDice: HTMLSelectElement = document.getElementById("input_number_dice") as HTMLSelectElement;
    const selectNumber = Number(inputNumberDice.value);

    switch (selectNumber) {
    case 1:
    case 2:
      dicePosition = "left";
      break;
    case 3:
    case 4:
      dicePosition = "center";
      break;
    default:
      dicePosition = "";
      break;
    }

    const options = {
            element: field
          , numberOfDice: selectNumber
          , callback: response
          , delay: 100000
      };

      rollADie(options);
  }
</script>

<div style="padding: 6px; text-align: right;">
  <div id="field_roll_dice" class="{dicePosition}"></div>
  <div class="result"><input type="text" readonly id="result_dice" class="nes-input is-error is-dark"></div>
  <div class="nes-select is-dark">
    <select id="input_number_dice">
      <option value="2" disabled selected hidden>ダイス数:デフォルト2</option>
      <option value="1">1</option>
      <option value="2" selected>2</option>
      <option value="3">3</option>
      <option value="4">4</option>
      <option value="5">5</option>
      <option value="6">6</option>
      <option value="7">7</option>
      <option value="8">8</option>
      <option value="9">9</option>
      <option value="10">10</option>
    </select>
  </div>
  <span class="nes-btn" on:click="{rollDice}">ダイスロール</span>
  <div id="result_message_roll_dice"></div>
</div>

<style lang="scss">
  #field_roll_dice {
    align-content: center;
    margin: 7px;
    height: 250px;
    width: 355px;
    background-color: #A70000;
    box-shadow: 3px 3px 10px 3px rgba(0,0,0,0.75) inset,-3px -3px 10px 0px rgba(0,0,0,0.75);
  }

  .result {
    margin: 2px 10px;
    float: left;
    width: 80px;

    input {
      font-size: 25px;
      text-align: right;
    }
  }

  .nes-select {
    float: left;
    margin-left: 30px;
    width: 100px;

    select {
      height: 45px;
    }
  }

  #result_message_roll_dice {
    clear: both;
    text-align: center;
    font-size: 22px;
  }
</style>
