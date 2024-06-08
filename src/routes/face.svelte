<script>

</script>
<div class="face-landing-page">
	<div class="profile-description">
		<h1>Vaibhav Khinvasara</h1>
		<p>Professional couch potato and enthusiastic brogrammer in Rust, Svelte, Django etc etc</p>
	</div>
	
	<div class="profile-image">
		<img src="/profile.jpg" alt="Vaibhav Khinvasara's Profile" />
	</div>	
</div>
<div class="technologies-worked-with">
	<div class="technologies">
		<h2>Technologies worked with:</h2>
	</div>
	<div class="technologies-images">
		<img src = "/django.svg" alt="Django" />
		<img src = "/rust.svg" alt="Rust" />
	</div>
</div>
<style>
	.face-landing-page {
		display: flex;
		justify-content: space-around;

		align-items: center;
		width: 90%;
		margin: 0.5rem auto;
		margin-top: 3rem;
	}

	.profile-description {
		width: 50%;
	}
	.profile-description h1, p {
		padding: 0.3rem;
	}
	.profile-image {
		width: 30%;
		height: 30%;
		border-radius: 50%;
		overflow: hidden;
	}

	.profile-image img {
		width: 100%;
	}

	@keyframes scroll{
		0% {
			transform: translateX(0);
		}
		100% {
			transform: translateX(calc(-250px*7));
		}
	
	}
	.technologies-worked-with {
		display: flex;
		justify-content: space-around;
		overflow-x: auto;
		align-items: center;
		width: 90%;
		margin: 0.5rem auto;
	}
	.technologies {
		width: 50%;
	}
	.technologies-images {
		display: flex;
		justify-content: flex-start;
		margin: 1rem;
		animation: scroll 40s linear infinite;
	}
	.technologies-images img{
		width: 250px;
		display: flex;
		justify-content: space-around;
	}
</style>
