<script>
  import { Application } from '@splinetool/runtime';
  import { onMount } from 'svelte';

  onMount( () => {
    // make sure you have a canvas in the body
    const canvas = document.getElementById('canvas3d');

    // change canvas height and width & color
    canvas.width = window.innerWidth;
    canvas.height = window.innerHeight;

    canvas.style.backgroundColor = "black";

    // start the application and load the scene
    const spline = new Application(canvas);
    spline.load('https://prod.spline.design/0D0JpB5DDQnMw2KH/scene.splinecode');
  });
</script>

<main>
  <canvas id="canvas3d"></canvas>
</main>

<style>
</style>