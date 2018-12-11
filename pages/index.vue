<template>
  <div>
    <div class="slider" data-slide="1">
      <div class="container"></div>
      <div class="temp">
        <div>
          <div>
            <h3>Крупы</h3>
            <p>Рассыпчатые традиционные каши остаются основным элементом здорового питания на протяжении веков. Богатые витаминами и минералами крупяные каши и сегодня станут незаменимым и любимым блюдом вашего стола!</p>
            <button>Узнать больше</button>
          </div>
          <img src="@/assets/pic/banner1.jpg" width="1920" height="469" alt="">
        </div>
        <div>
          <div>
            <h3>Сушки, баранки, пряники</h3>
            <p>Традиционно любимые сладости для детей и взрослых! Они создадут атмосферу домашнего тепла и уюта для семейного чаепития или встречи с друзьями.</p>
            <button>Узнать больше</button>
          </div>
          <img src="@/assets/pic/banner2.jpg" width="1920" height="469" alt="">
        </div>
        <div>
          <div>
            <h3>Слайсы, хлебцы</h3>
            <p>Слайсы и хлебцы – полноценная замена традиционному хлебу. Слайсы сделают ваше диетическое питание не только сбалансированным и полезным, но еще и разнообразным!</p>
            <button>Узнать больше</button>
          </div>
          <img src="@/assets/pic/banner3.jpg" width="1920" height="469" alt="">
        </div>
        <div>
          <div>
            <h3>Хлопья, палочки, подушечки</h3>
            <p>Сухие завтраки - идеальное начало дня! Они вкусные, питательные и изготовлены из натурального сырья. Кроме того, Вам совсем не нужно тратить время на их приготовление!</p>
            <button>Узнать больше</button>
          </div>
          <img src="@/assets/pic/banner4.jpg" width="1920" height="469" alt="">
        </div>
      </div>
    </div>
    <ul class="production" data-slide="2">
      <li class="col1" v-for="brand in brands">
        <div>
          <h3><a href="#">{{brand.name}}</a></h3>
          <p>{{brand.desc}}</p>
        </div>
      </li>

    </ul>
    <div class="introduction" data-slide="3">
      <h1>Продукты от ООО «Квантсервер» это:</h1>
      <div>
        <h5>Польза и безопасность</h5>
        <p>Мы постоянно осуществляем контроль качества продукции на всех стадиях производства (от выращивания сырья до упаковки и доставки), что подтверждается многочисленными сертификатами качества, и  используем только натуральные ингредиенты с плодородных полей Алтая.</p>
        <h5>Богатый выбор</h5>
        <p>Широкий ассортимент наших товаров обеспечивает здоровое сбалансированное питание, а для удобства использования мы предусмотрели различные варианты фасовок на все случаи жизни.</p>
        <h5>Точность и надежность</h5>
        <p>Отлаженная система логистики и транспортировки позволяет доставить свежую продукцию точно в срок.</p>
      </div>
    </div>
    <div class="quality" data-slide="4">
      <h2>Факты качества:</h2>
      <div>
        <ul class="jcarousel">
          <li><a href="@/assets/pic/poster.jpg" class="zoom" rel="g"><img src="@/assets/pic/fact1.jpg" width="139" height="140" alt=""></a></li>
          <li><a href="@/assets/pic/poster.jpg" class="zoom" rel="g"><img src="@/assets/pic/fact2.jpg" width="139" height="140" alt=""></a></li>
          <li><a href="@/assets/pic/poster.jpg" class="zoom" rel="g"><img src="@/assets/pic/fact3.jpg" width="139" height="140" alt=""></a></li>
          <li><a href="@/assets/pic/poster.jpg" class="zoom" rel="g"><img src="@/assets/pic/fact4.jpg" width="139" height="140" alt=""></a></li>
          <li><a href="@/assets/pic/poster.jpg" class="zoom" rel="g"><img src="@/assets/pic/fact5.jpg" width="139" height="140" alt=""></a></li>
          <li><a href="@/assets/pic/poster.jpg" class="zoom" rel="g"><img src="@/assets/pic/fact1.jpg" width="139" height="140" alt=""></a></li>
          <li><a href="@/assets/pic/poster.jpg" class="zoom" rel="g"><img src="@/assets/pic/fact2.jpg" width="139" height="140" alt=""></a></li>
          <li><a href="@/assets/pic/poster.jpg" class="zoom" rel="g"><img src="@/assets/pic/fact3.jpg" width="139" height="140" alt=""></a></li>
          <li><a href="@/assets/pic/poster.jpg" class="zoom" rel="g"><img src="@/assets/pic/fact4.jpg" width="139" height="140" alt=""></a></li>
          <li><a href="@/assets/pic/poster.jpg" class="zoom" rel="g"><img src="@/assets/pic/fact5.jpg" width="139" height="140" alt=""></a></li>
        </ul>
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
import Header_div from '~/components/Header.vue'
import Footer_div from '~/components/Footer.vue'


export default {
  head: {
    title: 'Главная'
  },
  components: {
    Header_div,
    Footer_div
  },
  data(){
    return {
      brands : [
        {
          'name': 'ТМ «Никитич»',
          'desc' : 'Вкус кукурузных палочек «Никитка» давно знаком и любим многими покупателями с детства!'
        },
        {
          'name': 'Палыч',
          'desc' : 'Вкус кукурузных палочек «Никитка» давно знаком и любим многими покупателями с детства 2!'
        },

      ]
    }
  }
}
</script>
