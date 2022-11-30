<svelte:head>
	<title>About</title>
	<meta name="description" content="About this app" />
</svelte:head>

<div class="text-column">
	
	I completed my master's degree in Aalto University in Summer of 2022

	<ul>
		<li>Aalto University, School of Science, Masters programme in Life Science Technologies</li>
		<li>Major in Bioinformatics and digital health.</li>
		<li>Master Thesis: Deep Learning Methodologies in Drug Target prediction
			<ul> 
				<li>The thesis studied recurrent convolutional neural networks in drug discovery and introduced new model for predicting potential interactions between drug molecules and group of proteins known as kinases.</li>
				<li> Grade 4/5 </li>
				<li>  <a href="https://aaltodoc.aalto.fi/handle/123456789/116273"> Archived here </a> </li>
				<li>  <a href="https://github.com/serveri24h/ThesisResultsReplication"> Repository for replicating results here </a> </li>
			</ul>
		</li>
	</ul>

	<p> Courses that I consider the most important pieces of my degree </p>

	<table>
		<tr><th>Course Name</th><th>Degree</th><th>University</th><th>Grade</th></tr>
		<tr><td>Machine Learning</td><td>MSc</td><td>IST Técnico</td><td>16/20</td></tr>
		<tr><td>Artificial Intelligence and Decision Systems</td><td>MSc</td><td>IST Técnico</td><td>14/20</td></tr>
		<tr><td>Machine Learning in Bioinformatics</td><td>PhD/MSc</td><td>Aalto</td><td>4/5</td></tr>
		<tr><td>Life Science Technologies Project Course <br> Project: Microarray data analysis with machine learning models</td><td>PhD/MSc</td><td>Aalto</td><td>4/5</td></tr>
		<tr><td>Modeling Biological Networks</td><td>PhD/MSc</td><td>Aalto</td><td>3/5</td></tr>
		<tr><td>Computational Biology</td><td>MSc</td><td>IST Técnico</td><td>15/20</td></tr>
		<tr><td>High-Throughput Bioinformatics</td><td>PhD/MSc</td><td>Aalto</td><td>3/5</td></tr>
		<tr><td>Bayesian Data Analysis</td><td>PhD/MSc</td><td>Aalto</td><td>3/5</td></tr>
		<tr><td>Information Systems and Databases</td><td>MSc</td><td>IST Técnico</td><td>14/20</td></tr>
		<tr><td>Experimental and Statistical Methods in Biological Sciences</td><td>MSc</td><td>Aalto University</td><td>3/5</td></tr>
	</table>

	<p> Before transfering into more computational and data driven domain, my journey in university started by studying chemical engineering. Although I was interested in the field, I felt like chemistry was not what I wanted to do for the rest of my life. Once I got my bachelor's degree, I decided to apply for a master's programme in bioinformatics. When I first started studying bioinformatics, I was overwhelmed by the computer science part of the programme. I had to study extra to understand the prerequisites, but once I got there I fell in love with computing, machine learning, and programming in general. I was particularly interested in deep learning and wrote neural network algorithms from scracths several times just understand the algorithm as compehensively as possible and finally wrote my master's about deep learning methodologies in drug kinase prediction. And although there is lot of room to do better and the code is somewhat messy, I'm quite happy with my thesis.</p>

</div>



<style>

	.text-column {
		display: flex;
		align-items: left;
	}

	ul, li {
		color: #b0b0b0;
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

		list-style: none;
	}

	a {
		color: #f0f0f0;
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

</style>
