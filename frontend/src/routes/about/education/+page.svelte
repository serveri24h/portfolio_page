<svelte:head>
	<title>About</title>
	<meta name="description" content="About this app" />
</svelte:head>

<div class="text-column">
	<h1> Education </h1>
	<div class="text-field">
		<p>I graduated with a master's degree in Aalto University in Summer of 2022. This page lists more detailed information about my studies.</p>

		<ul>Aalto University, School of Science, Masters programme in Life Science Technologies
			<li>Major in Bioinformatics and digital health.</li>
			<li>Master Thesis: Deep Learning Methodologies in Drug Target prediction
				<ul> 
					<li> Grade: 4/5 </li>
					<li>  <a href="https://aaltodoc.aalto.fi/handle/123456789/116273"> Archived here </a> </li>
					<li>  <a href="https://github.com/serveri24h/ThesisResultsReplication"> Repository for replicating results here </a> </li>
					<li class="smaller-text">The thesis studied recurrent convolutional neural networks in drug discovery. It also introduced a new model for predicting potential interactions between drug molecules and group of proteins known as kinases.</li>
				</ul>
			</li>
		</ul>
	</div>

	<div class="text-field">
		<p> Courses that I consider the most important pieces of my degree are listed below. Some of the courses were completed during the Erasmus exchange period in Lissabon's technical University, IST Técnico.</p>
		<div class="table-div">
			<table>
				<tr><th>Course Name</th><th>University</th><th>Grade</th></tr>
				<tr><td>Machine Learning</td><td>IST Técnico</td><td>16/20</td></tr>
				<tr><td>Artificial Intelligence and Decision Systems</td><td>IST Técnico</td><td>14/20</td></tr>
				<tr><td>Machine Learning in Bioinformatics</td><td>Aalto</td><td>4/5</td></tr>
				<tr><td>Life Science Technologies Project Course <br> Project: Microarray data analysis with machine learning models</td><td>Aalto</td><td>4/5</td></tr>
				<tr><td>Modeling Biological Networks</td><td>Aalto</td><td>3/5</td></tr>
				<tr><td>Computational Biology</td><td>IST Técnico</td><td>15/20</td></tr>
				<tr><td>High-Throughput Bioinformatics</td><td>Aalto</td><td>3/5</td></tr>
				<tr><td>Bayesian Data Analysis</td><td>Aalto</td><td>3/5</td></tr>
				<tr><td>Information Systems and Databases</td><td>IST Técnico</td><td>14/20</td></tr>
				<tr><td>Experimental and Statistical Methods in Biological Sciences</td><td>Aalto University</td><td>3/5</td></tr>
			</table>
		</div>
	</div>
	<div class="text-field">
		<p> My journey in university started by studying chemical engineering. Although I was interested in the field, I felt like chemistry was not what I wanted to do for the rest of my life. Once I got my bachelor's degree, I decided to apply for a master's programme in bioinformatics, which has served as a bridge to more computatinal on data driven understanding.</p>
		<!--p>When I first started studying bioinformatics, I was overwhelmed by the computer science part of the programme. I had to study extra to understand the prerequisites, but once I got there I fell in love with computing, machine learning, and programming in general. I was particularly interested in deep learning and wrote neural network algorithms from scracths several times just understand the algorithm as compehensively as possible and finally wrote my master's about deep learning methodologies in drug kinase prediction. And although there is lot of room to do better and the code is somewhat messy, I'm quite happy with my thesis.</p-->
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
		padding-top: 1em;
		padding-left: 1.5em;
		list-style: none;
	}

	ul li ul {
		padding-top: 10px;
	}

	td, th {
		border: solid 1px #ffffff;
		padding: 0.5em;
	}

	td {
		font-size: small;
		height: 3em;
	}

	th {
		background-color: rgba(127, 11, 11, 0.5);
	}

	a {
		color: #ffffff;
	}

	.table-div {
		padding-top: 1em;
		display: flex;
		flex-direction: column;
		width: 100%;
		align-items: center;
	}

</style>
