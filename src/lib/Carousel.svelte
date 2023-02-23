<script>
// @ts-nocheck
	import { fly } from 'svelte/transition';
	import { quintOut } from 'svelte/easing';
	import Siema from 'siema';
	let flag = true;
	function rotateContentLeft() {
		flag = !flag;
	}
</script>

<div class="buttonContainer">
        <!-- svelte-ignore a11y-click-events-have-key-events -->
        <div class="buttonLeft"/>
        <div class="buttonRight" />
</div>
<div class="frameContainer">
		<div class="currentItem" />
<!-- 
	{#if flag}
		<div class="currentItem" in:fly="{{x: 5000}}" out:fly="{{x: -1000, duration:2000}}"/>
	{/if}   -->
</div>



<style>
	.buttonContainer {
		position: fixed;
		top: 35%;
		width: 100%;
		height: 30%;
		z-index: 2;
	}

	.buttonLeft {
        position: fixed;
        top: 46%;
        left: 2%;
		width: 0;
		height: 0;
		border: 6vh solid transparent;
		border-right: 5vw solid rgba(255, 255, 255, 0.3);
        border-radius: 6%;
	}

    .buttonRight {
        position:fixed;
        top: 46%;
        right: 2%;
		width: 0;
		height: 0;
		border: 6vh solid transparent;
		border-left: 5vw solid rgba(255, 255, 255, 0.3);
        border-radius: 6%;
	}

	.frameContainer {
		margin-top: 10%;
		margin-right: 50%;
		width: 100%;
		height: 100%;
		display: grid;
		grid-gap: 20%;
	}
	.currentItem {
		border: 2px solid transparent rgba(255, 255, 255, 0.5);
		border-radius: 5px;
		background-color: rgba(255, 255, 255, 0.5);
		height: 50%;
		width: 30%;
		margin-left: auto;
		margin-right: auto;
	}
</style>
