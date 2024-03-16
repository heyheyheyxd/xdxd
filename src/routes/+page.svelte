<svelte:head>
    <title>Магазин Дмитрия Усимова</title>
</svelte:head>

<div class="container">
    <div class="info">
        <div class="animate-background">
            <div class="container info-container">
                <div class="info-text">
                    <h1>
                        <p class="animate-text-1">Добро пожаловать в магазин</p>
                        <p class="text-2">Дмитрия Усимова</p>
                    </h1>
                </div>
                <h2 class="subtitle">
                    У нас вы найдете лучшие товары по выгодным ценам!
                </h2>
                <div style='color:black' class='scroll-button animate-scroll'>
                    <a href='/catalog'>Посмотреть каталог</a>
                    <div class='arrow'></div>
                </div>
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
        margin: 50px auto;
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
        font-weight: 800;
        letter-spacing: -0.03em;
    }

    .info h2 {
        max-width: 65ch;
        font-weight: 200;
        margin-top: 0.50rem;
    }
    
    .background-div {
        background-color: #f8f9fa; /* Используем пастельный цвет фона */
        width: 100%;
        height: 56vh;
        margin: -160px auto;
    }
</style>

