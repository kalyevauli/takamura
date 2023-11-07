<template>
  <div>
    <header id="header">
      <div class="container">
        <div class="header">
          <div class="circle">
            <h1>tak <br>am <br> ura</h1>
          </div>
          <div class="card relative z-2">
            <Menubar :model="items" />
          </div>
          <div class="ion">
            <a href="#">+7(499)112-38-17</a>
            <i class="pi pi-user" style="color: orange" />
            <i class="pi pi-instagram" style="color: orange" />
            <i class="pi pi-youtube" style="color:orange " />
            <i class="pi pi-whatsapp" style="color: orange" />
          </div>
        </div>
      </div>
    </header>
    <section id="hero">
      <div class="container">
        <div class="hero">
          <div class="hero-text">
            <ul>
              <li>
                <NuxtLink to="/event"> <h1>Роллы  <span>TAKAMURA</span></h1></NuxtLink>
              </li>
            </ul>
            <p>У нас есть особая любовь к авокадо,и поэтому <br> мы заворачиваем роллы в него и добавляем в начинку. <br>Авокадо много не бывает.</p>
            <h2>НАШ НОВЫЙ АДРЕС</h2>
            <h5>Производственная 12к1 «Порт Пивных Дегустаторов»</h5>
            <div class="card">
              <div class="flex flex-wrap align-items-center justify-content-center card-container blue-container">
                <div class="fadeinleft animation-duration-3000 animation-iteration-infinite flex align-items-center justify-content-center
         font-bold bg-orange-500 text-white border-round m-2 px-5 py-3">
                  Что ещё?
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section id="block">
      <div class="container">
        <div class="grid">
          <div class="col-6">
            <img src="/img/img.png" alt="img">
          </div>
          <div class="col-6" style="align-items: end">
            <h1>Мы выбираем <span>качественные</span> морепродукты,соединяем их со <span>свежайшими</span> овощами и добавляем немного о риса.</h1>
          </div>
        </div>
      </div>
    </section>
    <section id="class">
      <div class="container">
        <div class="class">

        </div>
      </div>
    </section>
    <div class="navbar">
      <Header/>
      <Header/>
      <Header/>
      <Header/>
    </div>
    <div class="navbar">

      <Header/>
      <Header/>
      <Header/>
      <Header/>
    </div>
  </div>
</template>
<script setup lang="ts">
const items = ref([
  {
    label: 'Hабор'
  },
  {
    label: 'Суши'
  },
  {
    label: 'Роллы'
  },
  {
    label: 'Теплые роллы'
  },
  {
    label: 'Маки'
  },
  {
    label: 'Салаты'
  },
  {
    label: 'Напитки'
  },
  {
    label: 'Соусы'
  }
])
</script>
