<template>
	<div id="app">

		<!-- Prob move transition logic inside child -->
		<navbar/>

		<router-view class="page" style="background-color: var(--bg-secondary)"/>
		
	</div>
</template>

<script>

import Navbar from './components/Navbar.vue'

export default {
	name: 'App',

	components: {
		Navbar
	},

	data: function() {
		return {
		}
	},


}
</script>

<style>
	:root {
		font-size: 16px;

		--text-primary: gray;
		--text-secondary: white;
		/*
		--bg-primary: #008080;
		--bg-primary-light: #139696;
		--bg-primary-dark: 	#006868;

		--bg-secondary: #0C2B74;
		--bg-secondary-dark: #07215D;
		*/
		--bg-primary: #FE3C73;
		--bg-primary-light: #FD1054;
		--bg-primary-dark: 	#FE6792;

		--bg-secondary: #FAB7B7;


		--navbar-width: 5rem;

		font-family: sans-serif;

		background-color: var(--bg-secondary);
	}

	html {
		max-width: 100%;
		overflow-x: hidden;
		overflow-y: scroll;
	}

	body {
		margin: 0;
		padding: 0;
	}

	body::-webkit-scrollbar {
		width: 0.25rem
	}

	body::-webkit-scrollbar-track {
		background: darkgray;
	}

	body::-webkit-scrollbar-thumb {
		background: gray;
	}

	.page {
		margin-left: var(--navbar-width);
	}

</style>
