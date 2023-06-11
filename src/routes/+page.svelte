<script>

  let hhmmss = "";

  setInterval(() => {
    hhmmss = new Date().toLocaleTimeString();
  }, 1000);
	let color='pink';
	let name='Посетитель сайта';
</script>

<lable for='name'>Имя</lable>
<input id='name' bind:value={name}>
<label for='color'>Цвет</label>
<input id='color' type='color' bind:value={color}>
<div style='background-color: {color}' class='swatch'/>
<h1 style='color: {color}'>Привет {name}!</h1>

<div>
	 I will be a clock.
</div>
<span style='color: {color}'>{hhmmss}</span>

<style>
	.swatch {
		display: inline-block;
		height: 20px;
		width: 20px;
	}
</style>