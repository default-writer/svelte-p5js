<script>
	export let name;
	import * as p5 from "./p5";
	import { setup, draw } from "./sketch";
	window.setup = setup;
	window.draw = draw;
</script>

<style>
	h1 {
		color: purple;
	}
</style>

<h1>Hello {name}!</h1>
