<script>
	  import  LinkedinIcon  from '/linkedin.svg';
	  import GithubIcon from '/github.svg';

</script>

<nav class="navbar">
	<div class="navlinks">
		<a href="/">Home</a>
		<a href = "/about">Recent Work</a>
		<a href="/contact">Get in touch</a>
	</div>
	<div class="socials">
		<a href="https://www.linkedin.com/in/vaibhav-khinvasara-61830020b/"><img src={LinkedinIcon} alt="Linkedin"></a>
		<a href = "github.com/vkhinvasara"><img src={GithubIcon} alt="Github"></a>
	</div>
</nav>

<style>
	.navbar {
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 1rem 2rem;
	}

	.navlinks a {
		text-decoration: none;
		color: #333;
		margin-right: 1rem;
	}

	.socials img {
		width: 30px;
		height: 30px;
		margin-right: 1rem;
	}
</style>