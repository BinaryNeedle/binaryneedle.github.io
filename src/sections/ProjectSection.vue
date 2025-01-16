<script setup lang="ts">
import { ref } from 'vue';
import LanguageButton from '../components/LanguageButton.vue';
import appRekamMedis from '../assets/img/projects/appRekamMedis.png';
import mypertamina from '../assets/img/projects/mypertamina.png';
import dashboard_inven from '../assets/img/projects/dashboard_inven.png';

const timelineItems = ref([
  {
    projectName: 'Sistem Rekam Medis',
    heading: appRekamMedis,
    description: 'Aplikasi ini dirancang untuk mempermudah pengelolaan dan penyimpanan data rekam medis pasien secara digital. Meningkatkan efisiensi dalam akses informasi medis',
    lang: [
      { lang1: 1, text: 'Laravel' },
      { lang2: 2, text: 'MySQL' },
      { lang3: 3, text: 'Javascript' },
    ]
  },
  {
    projectName: 'My Pertamina',
    heading: mypertamina,
    description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.Lorem ipsum dolor sit amet consectetur adipisicing elit.',
    lang: [
      { lang1: 1, text: 'SolidJS' },
      { lang2: 2, text: 'GraphQL' },
    ]
  },
  {
    projectName: 'Sistem Inventaris Produk',
    heading: dashboard_inven,
    description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.Lorem ipsum dolor sit amet consectetur adipisicing elit.',
    lang: [
      { lang1: 1, text: 'Laravel' },
      { lang2: 2, text: 'MySQL' },
    ]
  }
]);
</script>

<template>
  <!-- Project Section Start -->
  <div class="container w-full h-fit py-10" id="project">
    <p class="text-4xl p-2 border-b-2 w-fit border-blue-700 text-center mx-auto rounded mb-5 font-bold">Latest Works</p> <!-- Tambahkan text-center dan mx-auto -->
    <section class="timeline">
      <ul>
        <li v-for="(item, index) in timelineItems" :key="index">
          <div :class="index % 2 === 0 ? 'timeline-content flex flex-row' : 'timeline-content flex flex-row-reverse'" class="gap-[150px]">
            <div class="heading-image flex flex-1 justify-center text-center glow pt-3 px-3 pb-5">
              <img :src="item.heading" alt="Heading Image" class=" w-full rounded p-0" />
            </div>
            <div class="description flex flex-1 flex-col justify-center text-left p-4">
              <h1 class="text-3xl mb-2">{{ item.projectName }}</h1>
              <p class="text-base leading-7 mb-4 font-light">{{ item.description }}</p>
              <LanguageButton :text="item.lang" />
            </div>
          </div>
        </li>
      </ul>
    </section>
</div>
  <!-- Project Section End -->
</template>

<style scoped>
.container {
  width: 100%;
}

.timeline {
  width: 100%;
  margin: 0 auto;
  position: relative;
}

.timeline ul {
  list-style: none;
  padding: 0;
}

.timeline ul li {
  padding: 20px;
  color: white;
  border-radius: 10px;
  margin-bottom: 20px;
}

.timeline .glow {
  background: black;
  box-shadow: 0 8px 100px 0 rgba(54, 54, 255, 0.7);
  backdrop-filter: blur( 10px );
  -webkit-backdrop-filter: blur( 9.5px );
  border-radius: 10px;
  border: 2px solid rgba(8, 0, 255, 0.5);

}

@media only screen and (min-width: 768px) {
  .timeline:before {
    content: "";
    position: absolute;
    top: 0;
    left: 50%;
    transform: translateX(-50%);
    width: 2px;
    height: 100%;
    background-color: gray;
  }

  .timeline ul li {
    width: 100%;
    position: relative;
    margin-bottom: 50px;
  }

  .timeline ul li:hover::before {
    background-color: aqua;
  }
  .timeline ul li:nth-child(even) {
    flex-direction: row-reverse;
  }
}
</style>