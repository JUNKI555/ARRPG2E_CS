<script>
	export let version = "0.01";
</script>

<h1><span class="first">アリアンロッド</span><span class="last">RPG</span><span class="number">2E</span></h1>
<h2>キャラクターシートエディタ ver:{version}</h2>

<style lang="scss">
	h1 {
		color: #ff3e00;
    position: relative;
    height: 2.5em;
    width: 10em;
    font-size: 2em;
    margin: 0 auto;
    background: url('data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" version="1.1" viewBox="0 0 24 24"><path fill="%23555555" d="M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M12,4A8,8 0 0,1 20,12A8,8 0 0,1 12,20A8,8 0 0,1 4,12A8,8 0 0,1 12,4M12,6A6,6 0 0,0 6,12A6,6 0 0,0 12,18A6,6 0 0,0 18,12A6,6 0 0,0 12,6M12,8A4,4 0 0,1 16,12A4,4 0 0,1 12,16A4,4 0 0,1 8,12A4,4 0 0,1 12,8Z" /></svg>') no-repeat 5.5em center;
    
    .first {
      position: absolute;
      top: 0;
      left: 0;
      color: #ff3e00;
    }

    .last {
      position: absolute;
      top: 1em;
      right: 3.1em;
      color: #fff;
    }

    .number {
      position: absolute;
      top: -0.25em;
      right: 0.2em;
      color: #6666FF;
      font-size: 2.5em;
    }
  }
  
  h2 {
    font-size: 1.2em;
  }
</style>
