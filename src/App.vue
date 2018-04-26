<template>
	<div class="container" id="app">
		<section class="hero">
		  <div class="hero-body">
		    <div class="container">
		      <h1 class="is-size-1">
		        {{msg}}
		      </h1>
		      <p>To get started, edit <code>./src/App.vue</code>.</p>
		    </div>
		  </div>
		</section>

		<div class="columns">
			<div class="column">
				<h2 class="is-size-3">Starter-kit includes:</h2>
				<ul>
					<li><a href="https://vuejs.org/">Vue - The Progressive JavaScript Framework<a></li>
					<li><a href="https://bulma.io/">Bulma - CSS framework based on Flexbox</a></li>
					<li><a href="https://prettier.io/">Prettier - Code formatter</a></li>
					<li><a href="https://parceljs.org/">Parcel - Web application bundler</a></li>
					<li><a href="https://eslint.org/">Eslint - Pluggable JavaScript linter</a></li>
				</ul>
			</div>
			<div class="column">
				<a v-on:click="counter += 1" class="button is-primary block">Click Me</a>				
		 		<p>The button above has been clicked {{ counter }} times.</p>
			</div>
		</div>
	</div>
</template>

<script>
const name = 'Miljan'

export default {
	name: 'app',
	data() {
		return {
			msg: 'Welcome to Parcel Vue App',
			counter: 0,
		}
	},
}
</script>

<style lang="css">
#app {
  color: #56b983;
}

.hero {
	text-align: center;
}

ul {
	list-style-type: circle;
	margin-left: 10px;
}

li {
	margin-left: 20px;
}

a {
	color: #56b983;
}

a:hover {
	color: #56b983;
	text-decoration: underline;
}
</style>
