<nav>
    <div class="nav-container">
        <a href="/" class="nav-logo" title="Back to home">Дмитрий Усимов</a>
        <div class="nav-links">
            {#each nav as link}
                {#if link.isShow}
                    <a href={link.href} class="link">{link.title}</a>
                    <span>&nbsp;&nbsp;&nbsp;</span>
                {/if}
            {/each}
        </div>
    </div>
</nav>

<div class="container">
    <h1>Добро пожаловать в магазин Дмитрия Усимова!</h1>
    <p>Мы рады приветствовать вас в нашем онлайн магазине, где вы можете найти широкий ассортимент качественных товаров по доступным ценам.</p>
    <p>Мы гордимся нашими товарными предложениями и уверены, что вы сможете найти здесь что-то для себя или своих близких.</p>
    <p>Мы постоянно обновляем наш ассортимент, чтобы предложить вам самые последние тренды и новинки рынка.</p>
    <p>Не забудьте заглянуть в наш каталог товаров, чтобы увидеть все наши предложения!</p>
</div>

<script>
    const nav = [
        {
            title: "О нас",
            href: "/routes/blog",
            isShow: true,
        },
        {
            title: "Каталог",
            href: "/routes/project",
            isShow: true,
        },
        {
            title: "Контакты",
            href: "/routes/contacts",
            isShow: true,
        },
    ];
</script>

<style>
    .container {
        max-width: 1400px;
        margin: 50px auto;
    }

    .container h1 {
        font-size: 2rem;
        margin-bottom: 20px;
        color: #333;
    }

    .container p {
        font-size: 1.2rem;
        margin-bottom: 20px;
        color: #666;
    }

    .nav-container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 10px 20px;
        background-color: #ffffff;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        z-index: 1000;
    }

    .nav-logo {
        font-size: 1.5rem;
        font-weight: bold;
        color: #333;
        text-decoration: none;
    }

    .nav-links {
        display: flex;
        align-items: center;
    }

    .link {
        margin-left: 20px;
        color: #333;
        text-decoration: none;
        transition: color 0.3s ease;
    }

    .link:hover {
        color: #007bff;
    }
</style>
