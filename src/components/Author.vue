<template>
	<div class="author">

		<h1 Fresh Thoughts
		</h1>

		<p class="author__intro">
			A blog by Abhiraj Bhowmick. Discuss and reflect on life's greater questions.
		</p>

		<p class="author__links">
			<a href="//twitter.com/rainboestrykr">Follow on Twitter</a>
			<a href="https://abhirajbhowmick.hashnode.com">Read my Dev Blog</a>
		</p>

	</div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
export default {
	props: ['showTitle']
}
</script>

<style lang="scss">
.author {
	margin: 0 auto;
	max-width: 500px;
	text-align: center;
	padding-bottom: calc(var(--space) / 2);

	&__image {
		border-radius: 100%;
		width: 90px;
		height: 90px;
		margin-bottom: 1em;
	}

	&__intro {
		opacity: .8;
	}

	&__site-title {
		margin: 0 auto;
		font-size: 1.5em;
		max-width: 400px;
	}

	&__links {
		margin-top: -.5em;
		a {
			margin: 0 .5em;
		}
	}
}
</style>
