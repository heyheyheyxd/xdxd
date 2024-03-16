<script>
    // Создадим массив с тестовыми товарами
    let products = [
        {
            id: 1,
            name: 'Футболка',
            description: 'Красная футболка с логотипом',
            price: 500,
        },
        {
            id: 2,
            name: 'Джинсы',
            description: 'Синие джинсы прямого кроя',
            price: 1000,
        },
        {
            id: 3,
            name: 'Кроссовки',
            description: 'Белые кроссовки Adidas',
            price: 1500,
        },
        // Добавьте больше товаров по аналогии
    ];

    // Функция для добавления товара в корзину
    function addToCart(productId) {
        // В реальном приложении здесь будет логика добавления товара в корзину
        alert(`Товар с ID ${productId} добавлен в корзину`);
    }
</script>

<!-- Отображение каталога -->
<div class="catalog">
    {#each products as product}
        <div class="product">
            <h2>{product.name}</h2>
            <p>{product.description}</p>
            <p>Цена: {product.price} руб.</p>
            <button on:click={() => addToCart(product.id)}>Добавить в корзину</button>
        </div>
    {/each}
</div>

<style>
    /* Стили для каталога */
    .catalog {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
        gap: 20px;
    }

    .product {
        border: 1px solid #ccc;
        border-radius: 5px;
        padding: 20px;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    .product h2 {
        margin-bottom: 10px;
    }

    .product button {
        padding: 8px 12px;
        border-radius: 5px;
        background-color: #007bff;
        color: #fff;
        border: none;
        cursor: pointer;
        transition: background-color 0.3s;
    }

    .product button:hover {
        background-color: #0056b3;
    }
</style>

