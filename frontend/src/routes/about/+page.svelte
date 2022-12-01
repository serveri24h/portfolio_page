<script>

import HeaderTemplate from "../components/header/HeaderTemplate.svelte";

let data = [
		{
			url: '/about/education',
			name: 'Education',
			children: null,
		},
		{
			url: '/about/skills',
			name: 'Skills',
			children: null,
		},
	]

	
</script>

<svelte:head>
	<title>About</title>
	<meta name="description" content="About this app" />
</svelte:head>

<div class="text-column">
	<h1>Whoami</h1>
	<p>
		Greetings, I am a bioinformaticians and aspiring software engineer looking for job opportunities. I have created this page as portfolio project and to learn more about frontend development and deploying websites. If your company is looking for a software or data engineer, consider reading more about my degree or what skills i can provide and learn if necessary. 
	</p>
	<div class="redirect-div">
		<HeaderTemplate nav_data={data}/>
		
	</div>

	

	<h3>What am I looking for from an employer?</h3>
	<p>
		I'm mainly looking for an interesting job where I can solve problems. Although that is a very general answer, I get enthusiastic about different things very easily as long as they can provide me with challenges and ways to develop myself further. Therefore, it can be anything from implementing machine learning approaches to systems programming or frontend development. Depending on the assignment, I might require a short learning period. However, I stayed in the previous company that I worked for ten years (during which time the owner and the name changed three times), so I'm not a guy who jumps between jobs easily.
	</p>
	
</div>



<style>

	.redirect-div {
		display: flex;
		flex-direction: row;
		justify-content: space-around;
		height: 6.5em;
		--background: var(--backbone-color);
		padding-top: 2em;
	}

	h1, h3 {
		display: flex;
		flex-direction: row;
		justify-content: left;
	}

</style>
