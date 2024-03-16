<nav>
    <div class="nav-container">
        <a href="/" class="nav-logo" title="Back to home">heyheyhey shop</a>
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



<script>
    const nav = [
        {
            title: "Главная",
            href: "/about",
            isShow: true,
        },
        {
            title: "О нас",
            href: "/blog",
            isShow: true,
        },
        {
            title: "Каталог",
            href: "/project",
            isShow: true,
        },
        {
            title: "Контакты",
            href: "/contacts",
            isShow: true,
        },
    ];
</script>

<style>

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
