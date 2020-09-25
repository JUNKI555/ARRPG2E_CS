<script lang="ts">
	import ProfileImage from './ProfileImage.svelte';
</script>

<ProfileImage/>

<div class="nes-table-responsive">
  <table class="nes-table is-bordered is-dark"> 
    <tbody>
      <tr>
        <td colspan="2">
          <div class="nes-field">
            <label for="input_character_name">キャラクター名</label>
            <input type="text" id="input_character_name" class="nes-input is-dark" size="45">
          </div>
        </td>
      </tr>
      <tr>
        <td>
          <div class="nes-field is-inline">
            <label for="input_age">年齢</label>
            <input type="text" id="input_age" class="nes-input is-dark">
          </div>
        </td>
        <td>
          <div class="nes-field is-inline">
            <label for="input_sex">性別</label>
            <input type="text" id="input_sex" class="nes-input is-dark" size="1">
          </div>
        </td>
      </tr>
      <tr>
        <td>
          <div class="nes-field">
            <label for="input_player_name">プレイヤー名</label>
            <input type="text" id="input_player_name" class="nes-input is-dark">
          </div>
        </td>
        <td>
          <div class="nes-field">
            <label for="input_growth_point">使用成長点</label>
            <input type="text" id="input_growth_point" class="nes-input is-dark" size="20">
          </div>
        </td>
      </tr>
    </tbody>
  </table>
</div>

<style lang="scss">

</style>
