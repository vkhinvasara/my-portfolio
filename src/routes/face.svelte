<script>
    import { onMount } from 'svelte';
    import { Splide } from '@splidejs/splide';
    import { AutoScroll } from '@splidejs/splide-extension-auto-scroll';
	import '@splidejs/splide/dist/css/splide.min.css';

    let splide;

    onMount(() => {
        splide = new Splide('.technologies-images', {
            type: 'loop',
            drag: 'free',
            focus: 'center',
            perPage: 3,
            autoScroll: {
                speed: 1,
            },
        });

        splide.mount({ AutoScroll });
    });
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
<Splide aria-label="My Favorite Images">
<div class="technologies-worked-with">
    <div class="splide technologies-images">
        <div class="splide__track">
            <ul class="splide__list">
                <li class="splide__slide"><img src="/django.svg" alt="Django" /></li>
                <li class="splide__slide"><img src="/rust.svg" alt="Rust" /></li>
                <li class="splide__slide"><img src="/actix.png" alt="Actix-web" /></li>
                <li class="splide__slide"><img src="/wasm.svg" alt="" /></li>
                <li class="splide__slide"><img src="/flask.svg" alt="" /></li>
            </ul>
        </div>
    </div>
</div>
</Splide>


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
		height: 250px;
		width: 60%;
		margin: 0.5rem auto;
	}
	
	.technologies-images {
		display: flex;
		justify-content: flex-start;
		margin: 1rem;
		animation: scroll 40s linear infinite;
	}
	.technologies-images img{
		margin: 1 rem;
		width: 250px;
		display: flex;
		justify-content: space-around;
	}
</style>

