<svelte:head>
	<title>About</title>
	<meta name="description" content="About this app" />
</svelte:head>
<script>
	// Array to keep track of visibility for each job info
    let showInfo = [false, false];

    // Function to toggle job info visibility
    function toggleInfo(n) {
        showInfo[n] = !showInfo[n];
    }
</script>

<div class="wrapper">
	<ul>
		<li>
			<h1>From where</h1>
			<p>
				I’m from Kullavik, right next to Gothenburg. Here I grew up with my Mother and Father which both were engineers at Chalmers.  I also have a little brother, Lucas. Here in Kullavik I went to the local school and studied from grade 0 up to 9th. Continuing from there I went to Nti Johanneberg and studied tech. More specifically with a focus on programming. Here was the first time that I got to hear the opera has offices in Gothenburg as you came to visit the school one day. After that I moved further away to Jönköping University. Here I study new media design which gave further skills in coding, design and business.  For my 5th semester I moved either further to Switzerland to study at FHNW and took courses within data science and informatic. After all this moving away from Gothenburg has made me want to get back <q>gammla goda göteborg</q> 
			</p>
		</li>
		<li>
			<h1>Career smart skills test</h1>
			<h3>The PDF</h3>
			<a href="docs/CareerTest.pdf">Press here to download</a>
			<h2>Reflection</h2>
			<p>I often see myself and as well receive feedback from others of me being the “glue” of the group. The results from this test seem to reinforce that perspective, and I consider it an important skill to develop further. Being the glue of the group to me, means helping everyone achieve a better and clearer understanding of the goals. Skills such as “not being defensive when others don’t agree” are crucial, as a poor group dynamic can lead to confusion and make implementing new ideas difficult. I know I like to make my voice heard, but just as important is understanding others’ perspectives. I see this as a highly desirable skill because it allows a team to develop with multiple perspectives and clarity. Of course not every time every one opinion can be used but then the importance of “Negotiating a win-win result” becomes more crucial. </p>
			<p>Although I often take on a leadership role when things are unclear, it’s not something I actively seek out it just tends to happen naturally. I feel confident in my ability to lead, but I prefer focusing on working with a team because I believe great leaders emerge from strong teams, rather than strong leaders creating great teams. According to the test results, leadership was a lower priority area for me, which makes sense, as I see myself prioritizing collaboration over directing.</p>
			<p>In my past summer jobs, I’ve been in leadership roles, and in many school projects, I end up as the unofficial leader. I believe it’s important to adapt to your role within the group and to play to your strengths. It’s also essential to recognize that you’re not the center of everything and to step back when others are more qualified to take the lead. However, if there’s a gap and no one else is willing to step up, I’m usually ready to take on that responsibility.</p>
		
		</li>
		<!-- <li>
			<h1>How I work</h1>
			<p>From this test I got that _____ which .....</p>
		</li> -->
		<li>
			<h1>Prevoius jobs</h1>
			<ul class="prevJobs">
				<li>
					<section>
						<h2>Landvetter</h2>
						<p>Prm Cordinator</p>
					</section>
					<p>In this roll, my work was to cordinat the staff that assist people with travel difficulties. The role aswell included to ensure the security on the airport with OPC(operation center). </p>
					<!-- <p class="jobInfo" style="display: {showInfo[0] ? 'block' : 'none'};"  >Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores odit eius perferendis sint placeat alias illum iusto, ipsum corporis, reiciendis tempora perspiciatis delectus, mollitia id modi error veritatis atque. Totam?</p>
					<button on:click={()=>toggleInfo(0)}>+</button> -->
				</li>
				<li>
					<section>
						<h2>Kappa bar</h2>
						<p>Bartender</p>
					</section>
					<p>
						Here, I was responsible for both working in the bar and ensuring timely ordering of new supplies.
					</p>
					<!-- <p class="jobInfo" style="display: {showInfo[1] ? 'block' : 'none'};">
						Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores odit eius perferendis sint placeat alias illum iusto, ipsum corporis, reiciendis tempora perspiciatis delectus, mollitia id modi error veritatis atque. Totam?</p>
						<button on:click={()=>toggleInfo(1)}>+</button> -->
				</li>
			</ul>
		</li>
		<li class="skills">
			<h1>Skills</h1>
			<ul>
				<li>Svelte</li>
				<li>Scss</li>
				<li>Node</li>
				<li>Javascripts</li>
				<li>Ruby</li>
				<li>SQlite</li>
				<li>Figma</li>
				<li>Photoshop</li>
				<li>Indesign</li>
				<li>Illustrator</li>
				<li>Powerpoint</li>
				<li>QMK</li>
				<li>Git</li>
				<li>CSS</li>
				<li>HTML</li>
				<li>Word</li>
				<li>Drivers license</li>

			</ul>
		</li>
		<li class="intresst">
			<h1>Intresst</h1>
			<ul>
				<li>Computers</li>
				<li>Video games</li>
				<li>Painting</li>
				<li>Mecchanical keyboards</li>
				<li>Vinyls</li>
				<li>Homebrewing cider</li>
				<li>Cooking</li>
			</ul>
		</li>
		<li>
			
		</li>
	</ul>
</div>
<style>
	li{
		list-style: none;
	}
	.prevJobs{
		display: flex;
		justify-content: space-around;
		width: auto;
		margin-right: 5%;
		flex-direction: column;
		gap: 2rem;
		
	}
	.prevJobs li{
		background-color: blanchedalmond;
		padding: 5%;
		background: rgba(255, 255, 255, 0.5);  
		backdrop-filter: blur(.15rem); 
		box-shadow: 0 4px 6px rgba(1, 1, 0, 0.2);
		border-top: .1rem rgba(255, 255, 255, 0.2) solid;
		text-align: left;
		padding: 0% 5%;
		text-decoration: none;
		letter-spacing: .5rem;
		width: fit-content;
		display: flex;
		gap: 2.5%;
		align-self: center;
	}
	.prevJobs li button{
		background-color: var(--felixPurple);
		color: var(--felixWhite);
		border: none;
		height: 2rem;
		width: 2rem;
		font-weight: bold;
		align-self: center;
	}
	.jobInfo {
	  	margin: 5%;
		letter-spacing: normal;
	}
	.skills ul, .intresst ul{
		display: flex;
		gap: 1rem;
		flex-wrap: wrap;
	}

	.skills ul li, .intresst li{ 
		background-color: var(--felixWhite);
		padding: 0.5rem;
		align-self: center;
		border: solid var(--felixPurple);
		
	}
    a{
		color: var(--felixPurple);
		background-color: var(--felixWhite);
		padding: .5rem;
		border: solid var(--felixPurple);
		
	}
	
</style>