<template>
    <div>
        <div class="content">
            <h1><span>Новости</span></h1>

            <div class="news">
                <div v-for="(post, index) in posts" :key="index">
                    <h6>18 августа 2014г.</h6>
                    <div>
                        <img src="@/assets/pic/news1.jpg" width="80" height="80" alt="">
                        <nuxt-link :to="~/posts/${post.id}">
                            {{ post.title }}
                        </nuxt-link>
                    </div>
                </div>


                <div class="pagination">
                    <div>
                        <p><a href="#">Начало</a></p>
                        <a href="#" class="prev"></a>
                        <ul>
                            <li><a href="#">1</a></li>
                            <li><a href="#">2</a></li>
                            <li><a href="#">3</a></li>
                            <li><a href="#">4</a></li>
                            <li><a href="#">5</a></li>
                            <li>...</li>
                        </ul>
                        <a href="#" class="next"></a>
                        <p><a href="#">Конец</a></p>
                    </div>
                </div>
            </div>
        </div>
        <div class="bottom">
            <a href="#"><img src="@/assets/pic/icon1.png" width="345" height="394" class="icon1" alt=""></a>
            <a href="#"><img src="@/assets/pic/icon2.png" width="392" height="439" class="icon2" alt=""></a>
            <a href="#"><img src="@/assets/pic/icon3.png" width="358" height="378" class="icon3" alt=""></a>
            <a href="#"><img src="@/assets/pic/icon4.png" width="371" height="405" class="icon4" alt=""></a>
        </div>
    </div>
</template>
<script>
    import axios from 'axios'

    export default {
        head: {
            title: 'Новости'
        },
        asyncData({ req, params }) {
            return axios.get('https://jsonplaceholder.typicode.com/posts')
                            .then((res) => {
                        return { posts: res.data.slice(0, 5) }
                    })
        }
    }
</script>