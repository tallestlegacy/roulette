<script>
	//const emojis = "😀😁😜😋🤯🥺".split("");

	const emojis = "supercalifragilisticexpialidocious".split("");
	let index = 0;
	$: emoji = emojis[index];

	function increment() {
		if (index < emojis.length - 1) {
			index++;
		} else {
			index = 0;
		}
	}
	setInterval(increment, 500);
</script>

<span>{emoji}</span>
<span>{index}</span>

<style>
	span {
		font-size: 10rem;
		font-family: "Courier New", Courier, monospace;
		color: darkturquoise;
		
	}
</style>
