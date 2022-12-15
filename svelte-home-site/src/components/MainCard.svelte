<script>
    import Card from "./Card.svelte"
</script>
    <section>
        <div>
        <Card>  
        <h1>I'm Simon Martin</h1>

        <h3>I'm a Japanese language student at Rochester Institute of Technology,
        interested in software engineering and web development</h3>
        </Card>
        </div>
</section>

<style>
    div{
        

    }
    section{
		min-height: 100vh;
		align-items: center;
		justify-content: center;
		display: flex;
        background-image: url("top-bg.png");
        margin: 0;
        object-fit: cover;
	}
</style>