<svelte:head>
<title>Фильмы</title>
</svelte:head>

<div class="container">
	<h1>Фильмы</h1>
    <div class="container-1">
	    <div class="apps">
		    {#each routes as page}
			    <div class="app">
				    <h2>{page.title}</h2>
				    <p><img src="{page.body}" alt="Чёт не работает"></p>
                    <div class="overview">
                        <h3 id="Description">{page.text}</h3>
                    </div>
			    </div>
		    {/each}
	    </div>
    </div>
</div>

<script>
    import { routes } from "./routes.js";
</script>
    
<style>
    
    .container {
        margin: 50px auto;
        max-width: 800px;
        padding: 0 20px;
    }

    .container-1 {
        margin: 50px auto;
        max-width: 600px;
    }
    
    .apps {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-gap: 20px;
    }
    
    .app {
        border: 1px solid #ddd;
        padding: 10px;
        box-shadow: 0 0 10px #eee;
        background-color: rgb(250, 240, 255);
        position: relative;
        overflow: hidden;
    }
    
    .link {
        color: rgb(10, 10, 139);
    }

    .overview {
    background-color: white;
    height: 330px;
    position: absolute;
    left: 0;
    bottom: 0;
    right: 0;
    max-width: 100%;
    transform: translateY(101%);
    transition: transform 0.3s ease-in;
    }

    .app:hover .overview{
    transform: translateY(0)
    }
</style>
    