<svelte:head>
	<title>About</title>
	<meta name="description" content="About this app" />
</svelte:head>

<div class="text-column">
	<h1>Skills</h1>
	<div class="text-field">
		<p>
			I consider myself more of a generalist rather than a specialist. Due to the interdisciplinary nature of my studies, I understand mathematics, computer science, machine learning, statistics, chemistry, and biology with varying level of sophistication. Although I'm not an expert in any of the mentioned fields, I'm an active learner who develops his skills every day.
		</p>
	</div>
	<div class="text-field">
		<h3>Computers</h3>
		<p> I have been programming with python for almost a decade now. Although my understanding about computer science and what happens under the hood was very shallow for a long time, programming in general was something that felt very natural to me. After graduation, I've been adopting new programing languages and improving my knowledge in web development, networking, systems programming and trying to understand computer as a whole down to the hardware level.</p>
		<p> Below are listed skills that I consider being my stronger suits: </p>
		<ul>
			<li> Machine learning, data-science and scientific computing with python and related libraries such as Pytorch, Numpy and Pandas. </li>
			<li> Bash scripting, Unix command line and related tools </li>
		</ul>
		<p> And some areas that where I'm getting more and more confident with and actively developing further: </p>
		<ul>
			<li> Rust </li>
			<li> Web Development (fullstack) </li>
			<li> Systems programming </li>
			<li> Networking </li>
		</ul>


	</div>
	<div class="text-field">
		<h3>Mathematics and Natural Sciences</h3>
		<p> Mathematics has been something that I have been always good at and enjoyed. I got full points (60/60) from math in Finnish matriculation examination (ylioppilaskokeet) and always enjoyed studying math in university. I'm confident that I have the tool kit to grasp even difficult concepts. I have also studied natural sciences from physics to chemistry and biology. </p>
	</div>
	<div class="text-field">
		<h3>Languages</h3>
		<p> I'm a native Finnish speaker and English is like a second language to me. I might make some grammar mistakes here and there, but I have know issue in communicating and documenting in English. In addition to English, I can also communicate and understand Swedish if necessary, Speak some Japanese and few phrases of Chinese. </p>
	</div>
</div>



<style>
		ul, li {
		color: var(--basic-text-color);
	}

	ul {
		font-weight: 600;
		display: flex;
		flex-direction: column;
		align-items: left;
	}

	li {
		font-weight: 300;
		padding: 0.5em;
		padding-left: 1.5em;
		list-style: disc;
	}

	ul li ul {
		padding-top: 10px;
	}
</style>
