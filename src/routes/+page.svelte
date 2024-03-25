<svelte:head>
    <title>Главная</title>
</svelte:head>

<div class="container">
    <div class="info">
        <div class="animate-background">
            <div class="container info-container">
                <div class="info-text">
                    <h1>
                        <p class="animate-text-1">Кинотеатр "Буревестник"</p>
                        <p class="text-2">Создатель сайта: Шаров Пётр Игоревич</p>
                    </h1>
                </div>
                <h2 class="subtitle">Сайт кинотеатра "Буревестник"</h2>
            </div>
        </div>
    </div>
</div>

<div class="background-div"></div>

<style>
    .info {
        text-align: center;
        position: relative;
    }

    .info-container {
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        text-align: left;
        align-items: start;
    }

    .container {
        max-width: 1400px;
        margin: 50px 0 0 2.5rem;
    }

    .info h1 {
        font-size: 4rem;
        margin: 0;
    }

    .info h1 p {
        position: relative;
        font: inherit;
        margin: 0;
        text-align: left;
        line-height: 130%;
        width: fit-content;
        font-weight: 750;
        letter-spacing: -0.03em;
    }

    .info h2 {
        max-width: 65ch;
        font-weight: 200;
        margin-top: 0.50rem;
    }
    
    .background-div {
        background-color: rgb(250, 240, 255);
        width: 100%;
        height: 5vh;
        margin: -60px auto;
    }
</style>