<template>
    <div>
        <div class="content">
            <h1><span>Новости {{page}}</span></h1>

            <div class="news">
                <div v-for="(post, index) in posts" :key="index">
                    <h6>18 августа 2014г.</h6>
                    <div>
                        <img src="@/assets/pic/news1.jpg" width="80" height="80" alt="">
                        <nuxt-link :to="'/news/'+post.id+'/'">{{ post.title }}</nuxt-link>
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
        <paginate-links for="posts" :show-step-links="true"></paginate-links>
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
    //import VuePaginateAl from 'vue-paginate-al'
    //import Pagination from 'vue-pagination-2';
    import VuePaginate from 'vue-paginate'


    export default {
        head: {
            title: 'Новости'
        },

        data(){
            return{
                page : 45,
                limit : 10,
                start : 1,
                paginate: ['posts']
            }
        },
        asyncData({ req, params }) {
            return axios.get('https://jsonplaceholder.typicode.com/posts')
                            .then((res) => {
                        return {
                            posts: res.data.slice(0, 10)

                        }
                    })
        },
        components : {
            //VuePaginateAl
            VuePaginate
        },
        methods : {
            goToFunction : function(page)
            {
                axios.get('https://jsonplaceholder.typicode.com/posts').then(res => {
                    this.posts = res.data.slice(10, 12);
                })
                .catch(e => {
                this.errors.push(e)
             })
            }
        }
    }
</script>