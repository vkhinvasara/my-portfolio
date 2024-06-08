<script>

</script>
<div class="face-landing-page">
	<div class="profile-description">
		<h1>Vaibhav Khinvasara</h1>
		<p>Professional couch potato and enthusiastic brogrammer in Rust, Svelte, Django etc etc</p>
	</div>
	
	<div class="profile-image">
		<img src="/profile.jpg" alt="Profile Picture" />
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
</style>
