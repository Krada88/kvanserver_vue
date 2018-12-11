<template>
    <div>
        <div class="content">
            <h1 v-if="error.statusCode === 404"><span>Страница не найдена</span></h1>
            <h1 v-else><span>Произошла ошибка</span></h1>
            <nuxt-link to="/">Вернуться на главную</nuxt-link>
         </div>
    </div>
</template>

<script>
    export default {
        props: ['error']
    }
</script>