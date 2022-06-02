<template>
  <div class="flex flex-wrap justify-center mt-[71px] gap-10">
    <div v-for="item in items" :key="item.id" class="flex justify-center gap-3 text-blue font-fontAlt w-4/12">
      <div>
        <img :src="`./src/assets/images/${item.img}`" :alt="item.title" class="h-[5rem] w-auto md:inline-block hidden">
      </div>
      <div class="lg:max-w-[390px] w-full ">
        <h2 class="font-bold text-3xl">{{ item.title }}</h2>
        <p class="font-light text-sm">{{ item.desc }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { id: 1, title: "Pendaftaran Mudah", desc: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s.", img: "image01.png" },
        { id: 2, title: "Tenaga Medis Profesional", desc: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s.", img: "image02.png" },
        { id: 3, title: "Proses Cepat", desc: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.", img: "image03.png" },
        { id: 4, title: "Tenaga Medis Profesional", desc: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.", img: "image02.png" },
      ]
    }
  }
}
</script>