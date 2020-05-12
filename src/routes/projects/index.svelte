<script context="module">
	export function preload({ params, query }) {
		return this.fetch(`blog.json`).then(r => r.json()).then(posts => {
			return { posts };
		});
	}
</script>

<script>
	export let posts;
</script>

<style>
	ul {
		margin: 0 0 1em 0;
		line-height: 1.5;
	}
</style>

<svelte:head>
	<title>
		Projects | Filip Holčík
	</title>
</svelte:head>

<section class="portfolio-block projects-cards">
	<div class="container">
		<div class="heading">
			<h2>My products</h2>
		</div>
		<div class="row">
			<div class="col-md-6 col-lg-4">
				<div class="card border-0"><a href="#"><img class="card-img-top scale-on-hover" src="assets/img/nature/image1.jpg" alt="Card Image"></a>
					<div class="card-body">
						<h6><a href="#">svelte-fullpage</a></h6>
						<p class="text-muted card-text">My first NPM module. Full page component for Svelte.</p>
					</div>
				</div>
			</div>
			<div class="col-md-6 col-lg-4">
				<div class="card border-0"><a href="#"><img class="card-img-top scale-on-hover" src="assets/img/nature/image2.jpg" alt="Card Image"></a>
					<div class="card-body">
						<h6><a href="#">svelte-lightbox</a></h6>
						<p class="text-muted card-text">My second NPM module. Lightweight lightbox component for Svelte.</p>
					</div>
				</div>
			</div>
			<div class="col-md-6 col-lg-4">
				<div class="card border-0"><a href="#"><img class="card-img-top scale-on-hover" src="assets/img/nature/image3.jpg" alt="Card Image"></a>
					<div class="card-body">
						<h6><a href="#">SmartCalc</a></h6>
						<p class="text-muted card-text">My first project, started as python 3 script and ended as Electron program.</p>
					</div>
				</div>
			</div>
			<div class="col-md-6 col-lg-4">
				<div class="card border-0"><a href="#"><img class="card-img-top scale-on-hover" src="assets/img/nature/image4.jpg" alt="Card Image"></a>
					<div class="card-body">
						<h6><a href="#">FIM Trade Pricing Tool</a></h6>
						<p class="text-muted card-text">My first proprietary program, business program for enterprise called "FIM Trade".</p>
					</div>
				</div>
			</div>
			<div class="col-md-6 col-lg-4">
				<div class="card border-0"><a href="#"><img class="card-img-top scale-on-hover" src="assets/img/nature/image5.jpg" alt="Card Image"></a>
					<div class="card-body">
						<h6><a href="#">FIM Trade website</a></h6>
						<p class="text-muted card-text">My first professional SSR website</p>
					</div>
				</div>
			</div>
			<div class="col-md-6 col-lg-4">
				<div class="card border-0"><a href="#"><img class="card-img-top scale-on-hover" src="assets/img/nature/image6.jpg" alt="Card Image"></a>
					<div class="card-body">
						<h6><a href="#">Fyto life website</a></h6>
						<p class="text-muted card-text">My first serious website.</p>
					</div>
				</div>
			</div>
		</div>
	</div>
</section>

<h1>Recent posts</h1>

<ul>
	{#each posts as post}
	<!-- we're using the non-standard `rel=prefetch` attribute to
				tell Sapper to load the data for the page as soon as
				the user hovers over the link or taps it, instead of
				waiting for the 'click' event -->
		<li><a rel='prefetch' href='blog/{post.slug}'>{post.title}</a></li>
	{/each}
</ul>