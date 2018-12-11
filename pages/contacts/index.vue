<template>
  <div>
    <div class="submenu contacts">
      <ul>
        <li class="active"><a href="#">Приемная</a></li>
        <li><a href="#">Финансовый отдел</a></li>
        <li><a href="#">Коммерческий отдел</a></li>
        <li><a href="#">Отдел снабжения</a></li>
        <li><a href="#">Отдел контроля качества</a></li>
        <li><a href="#">Отдел кадров</a></li>
      </ul>
    </div>
    <div class="content">
      <h1><span>Контакты</span></h1>
      <h2><span>Приемная</span></h2>
      <ul class="team">
        <li>
          <div>
            <img src="@/assets/pic/person1.jpg" width="178" height="178" alt="">
          </div>
          <h3>Перфильева<br> Татьяна<br> Юрьевна</h3>
          <h5>Секретарь</h5>
          <p>тел./факс +7 (3852) 32-52-83</p>
          <p>внутренний 101</p>
          <p>perfileva_ty@kvantserver.ru</p>
        </li>
        <li>
          <div>
            <img src="@/assets/pic/person2.jpg" width="178" height="178" alt="">
          </div>
          <h3>Дейкина<br> Алена<br> Александровна</h3>
          <h5>Финансовый директор</h5>
          <p>тел./факс +7 (3852) 32-52-82</p>
          <p>внутренний 155</p>
          <p>deykina_aa@kvantserver.ru</p>
        </li>
        <li>
          <div>
            <img src="@/assets/pic/person3.jpg" width="178" height="178" alt="">
          </div>
          <h3>Борисенко<br> Лариса<br> Владимировна</h3>
          <h5>Бухгалтер по расчету<br> с поставщиками и подрядчиками</h5>
          <p>тел./факс +7 (3852) 32-52-82</p>
          <p>внутренний 126</p>
          <p>borisenko_lv@kvantserver.ru</p>
        </li>
        <li>
          <div>
            <img src="@/assets/pic/person4.jpg" width="178" height="178" alt="">
          </div>
          <h3>Поварова<br> Анжелика<br> Жановна</h3>
          <h5>Директор по продажам</h5>
          <p>тел./факс +7 (3852) 32-52-84</p>
          <p>внутренний 143</p>
          <p>povarova_aj@kvantserver.ru</p>
        </li>
        <li>
          <div>
            <img src="@/assets/pic/person5.jpg" width="178" height="178" alt="">
          </div>
          <h3>Зайцев<br> Денис<br> Валерьевич</h3>
          <h5>Региональный менеджер <span>(Алтайский край, Новосибирская область, Красноярский край, страны ближнего зарубежья)</span></h5>
          <p>тел./факс +7 (3852) 32-52-84</p>
          <p>внутренний 140</p>
          <p>zaycev_dv@kvantserver.ru</p>
        </li>
      </ul>
      <div class="contacts">
        <ul>
          <li class="address">659318, Россия<br> Алтайский край, г. Бийск<br> ул. Яминская, 4а</li>
          <li class="phone">8 (3854) 32 - 52 - 83,<br> 32 - 52 - 84, 32 - 52 - 81</li>
          <li class="email"><a href="mailto:kvantserver@rambler.ru">kvantserver@rambler.ru</a></li>
        </ul>
        <div>
          <div>
            <script type="text/javascript" charset="utf-8" src="http://api-maps.yandex.ru/services/constructor/1.0/js/?sid=tjzIMgqov4iP4egsdYoIZVPFMdtZY_NX&width=627&height=315"></script>
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
import Logo from '~/components/Logo.vue'

export default {
	head: {
		  title: 'Контакты'
		},
  components: {
    Logo
  }
}
</script>
