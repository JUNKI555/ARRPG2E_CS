<script lang="ts">

</script>

<div>
  <div class="nes-table-responsive">
    <table class="nes-table is-bordered is-dark"> 
    <tbody>
      <tr>
        <td>
          <div class="nes-field is-inline">
            <label for="input_lv1_main_class">メインクラス</label>
            <input type="text" list="lv1_main_classes" id="input_lv1_main_class" class="nes-input is-dark" size="40">
            <datalist id="lv1_main_classes">
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
            <label for="input_lv1_support_class">サポートクラス</label>
            <input type="text" list="lv1_support_classes" id="input_lv1_support_class" class="nes-input is-dark">
            <datalist id="lv1_support_classes">
              <option value="ウォーリア"></option>
              <option value="アコライト"></option>
              <option value="メイジ"></option>
              <option value="シーフ"></option>
              <option value="アルケミスト"></option>
              <option value="ガンスリンガー"></option>
              <option value="サムライ"></option>
              <option value="サモナー"></option>
              <option value="セージ"></option>
              <option value="ダンサー"></option>
              <option value="ニンジャ"></option>
              <option value="バード"></option>
              <option value="モンク"></option>
              <option value="レンジャー"></option>
            </datalist>
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
