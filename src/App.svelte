<script>
	import P5Canvas from "./P5Canvas.svelte";
	export let name;

	let sketch1 = function(p5) {
		let x = 100;
		let y = 100;

		p5.setup = function() {
			p5.createCanvas(300, 200);
		};

		p5.draw = function() {
			p5.background(0);
			p5.fill(255);
			p5.rect(x,y,50,50);
		};
	};

	let sketch2 = function(p5) {
		let x = 100;
		let y = 50;
		
		p5.setup = function() {
			p5.createCanvas(300, 200);
		};

		p5.draw = function() {
			p5.background(0);
			p5.fill(255);
			p5.rect(x,y,50,50);
		};
	};

</script>

<style>
	h1 {
		color: purple;
	}
</style>

<h1>Hello {name}!</h1>
<P5Canvas id="p5canvas1" sketch={sketch1}/>
<P5Canvas id="p5canvas2" sketch={sketch2}/>