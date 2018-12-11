<template>
    <div class="header">
        <div>
            <div class="logo">
                <a href="/"><img src="@/assets/img/logo.png" width="113" height="114" class="big" alt=""></a>
                <a href="/"><img src="@/assets/img/logo_c.png" width="87" height="42" class="small" alt=""></a>
            </div>
            <div class="search">
                <button></button>
                <p><input type="text" placeholder="сушка Никитич"></p>
            </div>
            <div class="contacts">
                <h3><a href="tel:+73584325283">+7 3584 32 52 83</a></h3>
                <p>г. Бийск, Алтайский край</p>
            </div>
            <ul class="nav ln">
                <nuxt-link tag="li" to="/about/"><a>О компании</a></nuxt-link>
                <nuxt-link tag="li" to="/products/"><a>Продукция</a></nuxt-link>
                <nuxt-link tag="li" to="/news/"><a>Новости</a></nuxt-link>
            </ul>
            <ul class="nav rn">
                <nuxt-link tag="li" to="../"><a>Просто вкусно</a></nuxt-link>
                <nuxt-link tag="li" to="../"><a>Партнерам</a></nuxt-link>
                <nuxt-link tag="li" to="/contacts/"><a>Контакты</a></nuxt-link>
            </ul>
        </div>
    </div>
</template>