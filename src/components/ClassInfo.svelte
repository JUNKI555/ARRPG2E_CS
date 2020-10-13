<script lang="ts">

</script>

<div>
  <div class="nes-table-responsive">
    <table class="nes-table is-bordered is-dark"> 
    <tbody>
      <tr>
        <td>
          <div class="nes-field is-inline">
            <label for="input_main_class">メインクラス</label>
            <input type="text" list="main_classes" id="input_main_class" class="nes-input is-dark" size="40">
            <datalist id="main_classes">
              <option value="ウォーリア"></option>
              <option value="アコライト"></option>
              <option value="メイジ"></option>
              <option value="シーフ"></option>
            </datalist>
          </div>
        </td>
      </tr>
      <tr>
        <td>
          <div class="nes-field is-inline">
            <label for="input_support_class">サポートクラス</label>
            <input type="text" id="input_support_class" class="nes-input is-dark">
          </div>
        </td>
      </tr>
      <tr>
        <td>
          <div class="nes-field is-inline">
            <label for="input_secondary_support_class">第二サポート</label>
            <input type="text" id="input_secondary_support_class" class="nes-input is-dark">
          </div>
        </td>
      </tr>
      <tr>
        <td>
          <div class="nes-field is-inline">
            <label for="input_named_class">称号クラス</label>
            <input type="text" id="input_named_class" class="nes-input is-dark">
          </div>
        </td>
      </tr>
      <tr>
        <td>
          <div class="nes-field is-inline">
            <label for="input_family">種族</label>
            <input type="text" id="input_family" class="nes-input is-dark">
          </div>
        </td>
      </tr>
    </tbody>
    </table>
  </div>
</div>

<style lang="scss">
  .nes-field {
    > label {
      flex-grow: 4;
    }
  }
</style>
