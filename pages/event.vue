<template>
  <header id="header">
    <div class="container">
      <div class="header">
        <div class="circle">
          <h1>tak <br> am <br> ura</h1>
        </div>
        <div class="square">
          <NuxtLink to="/event"><a href="#">Наборы</a></NuxtLink>
          <a href="#">Суши</a>
          <a href="#">Роллы</a>
          <a href="#">Теплые роллы</a>
          <a href="#">Маки</a>
          <a href="#">Салаты</a>
          <a href="#">Напитки</a>
          <a href="#">Соусы</a>
        </div>
        <div class="ion">
          <a href="+7(499)112-38-17">+7(499)112-38-17</a>
          <i class=" pi pi-info-circle" style="color: orange"></i>
          <i class="pi pi-map" style="color: orange"></i>
          <i class="pi pi-shopping-cart" style="color: orange"></i>
          <i class="pi pi-bars" style="color:orange"></i>
        </div>
      </div>
    </div>
  </header>
 <div class="event">
   <div class="lux">
     <img src="/img/nabory.png" alt="img">
         <NuxtLink to="/"> <h1>LUX</h1></NuxtLink>
     <p>Калифорний с камчатским крабом <br> и манго,Дракон с креветкой, <br>Филадельфия люкс,Манго-авокадо <br>Вес:902г <br>Порция:32шт.</p>
     <div class="card" :style="{ position: 'relative', height: '50px' }">
       <SpeedDial :model="items" :radius="60" type="semi-circle" direction="up" :style="{ left: 'calc(5% - 2rem)', bottom: 0 }" />
       <Toast />
     </div>
   </div>
   <div class="lux">
     <img src="/img/nabory.png" alt="img">
     <NuxtLink to="/"> <h1>LUX</h1></NuxtLink>
     <p>Калифорний с камчатским крабом <br> и манго,Дракон с креветкой, <br>Филадельфия люкс,Манго-авокадо <br>Вес:902г <br>Порция:32шт.</p>
     <div class="card" :style="{ position: 'relative', height: '50px' }">
       <SpeedDial :model="items" :radius="60" type="semi-circle" direction="up" :style="{ left: 'calc(5% - 2rem)', bottom: 0 }" />
       <Toast />
     </div>
   </div>
   <div class="lux">
     <img src="/img/nabory.png" alt="img">
     <NuxtLink to="/"> <h1>LUX</h1></NuxtLink>
     <p>Калифорний с камчатским крабом <br> и манго,Дракон с креветкой, <br>Филадельфия люкс,Манго-авокадо <br>Вес:902г <br>Порция:32шт.</p>
     <div class="card" :style="{ position: 'relative', height: '50px' }">
       <SpeedDial :model="items" :radius="60" type="semi-circle" direction="up" :style="{ left: 'calc(5% - 2rem)', bottom: 0 }" />
       <Toast />
     </div>
   </div>
   <div class="lux">
     <img src="/img/nabory.png" alt="img">
     <NuxtLink to="/"> <h1>LUX</h1></NuxtLink>
     <p>Калифорний с камчатским крабом <br> и манго,Дракон с креветкой, <br>Филадельфия люкс,Манго-авокадо <br>Вес:902г <br>Порция:32шт.</p>
     <div class="card" :style="{ position: 'relative', height: '50px' }">
       <SpeedDial :model="items" :radius="60" type="semi-circle" direction="up" :style="{ left: 'calc(5% - 4rem)', bottom: 0 }" />
       <Toast />
     </div>
   </div>
 </div>
</template>
<script setup lang="ts">
import { ref } from 'vue'
import { useToast } from 'primevue/usetoast'
import { useRouter } from 'vue-router'

const toast = useToast()
const router = useRouter()

const items = ref([
  {
    label: 'Upload',
    icon: 'pi pi-plus',
    command: () => {
      router.push('/fileupload')
    }
  },
  {
    label: 'Vue Website',
    icon: 'pi pi-minus',
    command: () => {
      window.location.href = 'https://vuejs.org/'
    }
  }
])
</script>
