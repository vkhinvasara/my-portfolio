<script lang="ts">
   	import { onMount } from 'svelte';
    import { Splide, SplideSlide } from '@splidejs/svelte-splide';
    import { AutoScroll } from '@splidejs/splide-extension-auto-scroll';
    import '@splidejs/splide/dist/css/splide.min.css';

	
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

<div class="carosel">
<Splide aria-label = "Tech Stack" options={{autoplay: true, interval: 1000, pauseOnHover: false, perPage: 2, gap: '1rem', autoWidth: true, arrows: false, pagination: false}}>
	<SplideSlide>
		<img src="/rust.svg" alt="Rust" />
	</SplideSlide>
	<SplideSlide>
		<img src="/actix.png" alt="Actix-Web" />
	</SplideSlide>
	<SplideSlide>
		<img src="/django.svg" alt="Django" />
	</SplideSlide>
	<SplideSlide>
		<img src="/flask.svg" alt="Flask" />
	</SplideSlide>
	<SplideSlide>
		<img src="/wasm.svg" alt="Wasm" />
	</SplideSlide>
	<SplideSlide>
		<img src="/svelte.svg" alt="Svelte" />
	</SplideSlide>
	<SplideSlide>
		<img src="/react.svg" alt="React" />
	</SplideSlide>
	<SplideSlide>
		<img src="/solidity.svg" alt="Solidity">
	</SplideSlide>
</Splide>
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
	
	.carosel{
		display: flex;
		overflow-x: hidden;
		overflow-y: hidden;
		width: 60%;
		overflow-x: auto;
		white-space: nowrap;
		height: auto;
		align-items: center;
		justify-content: center;
		margin:auto;
	}
	.carosel img{
		width: 100px;
		height: auto;
	}

	
</style>

