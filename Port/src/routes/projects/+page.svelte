<script>

</script>
<div class="wrapper">
    <h1>Projects</h1>
    <section class="lanceyFoux">
        <h2>Lancey Foux album page</h2>
        <section class="imgSec">
            <img src="images/proj/lancey/lanceyHome.jpeg" alt="Homepage of Lancey Foux">
            <img src="images/proj/lancey/lanceyAlbums.jpeg" alt="Albums page of Lancey Foux">
            <img src="images/proj/lancey/lanceySongs.jpeg" alt="Songs page of Lancey Foux">
        </section>
        <section class="textSec">
            <p>A small project of an artist webpage of albums and songs. Made with Node Express, Javascript, Handlebars, SQlite, SCSS</p>
            <a href="https://github.com/Life-of-Felix/final-project-lancey-foux">Github</a>
        </section>
        
    </section>
</div>
<style>
    section img{
        width: 30%;
    }
    .lanceyFoux{
        background: rgba(255, 255, 255, 0.2);  
		backdrop-filter: blur(.15rem); 
		box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
		border-top: .1rem rgba(255, 255, 255, 0.2) solid;
    }
    .lanceyFoux h2{
        margin: 0% 5%;
        padding-top: 2.5%;
    }
    .imgSec{
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        padding: 2.5%;
    }
    .textSec{
        padding: 2.5%;
    }
    .textSec a{
        color: var(--felixPurple);
        padding: 1%;
        border: solid var(--felixPurple);
        text-decoration: none;
    }

</style>