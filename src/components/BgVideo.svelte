<div class="fullscreen-bg">
	<video class="fullscreen-bg__video" loop muted autoplay>
		<source src="../static/ehlen-analytics.mp4" type="video/mp4" />
	</video>
</div>

<style>
	.fullscreen-bg {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		z-index: -1;
		overflow: hidden;
	}

	.fullscreen-bg__video {
		min-width: 100vw;
		min-height: 100vh;
		width: auto;
		height: auto;
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
	}
</style>
