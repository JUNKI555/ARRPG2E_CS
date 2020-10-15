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
            <input type="text" list="list_main_class" id="input_main_class" class="nes-input is-dark" size="40">
            <datalist id="list_main_class">
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
            <input type="text" list="list_support_class" id="input_support_class" class="nes-input is-dark">
            <datalist id="list_support_class">
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
            <input type="text" list="list_family" id="input_family" class="nes-input is-dark">
            <datalist id="list_family">
              <option value="ヒューリン"></option>
              <option value="エルダナーン"></option>
              <option value="ネヴァーフ"></option>
              <option value="フィルボル"></option>
              <option value="ヴァーナ"></option>
              <option value="ドゥアン"></option>
              <option value="アーシアン"></option>
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
