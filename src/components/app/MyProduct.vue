<template>
  <div v-for="paket in pakets" :key="paket.id"
    class="px-4 py-4 mt-[64px] w-[100] md:w-[150px] md:h-[240px] lg:w-[240px] lg:h-auto border border-darkBlue font-fontAlt text-darkBlue rounded-lg">
    <img :src="`./src/assets/images/${paket.img}`" class="w-full" alt="...">
    <h2 class="font-bold text-lg md:text-base mt-3 leading-4">{{ paket.jenis }}</h2>
    <p class="font-light text-base lg:text-[8px] md:text-[8px] leading-normal my-2">{{ paket.desc }}</p>
    <div class="flex my-2">
      <img src="../../assets/icons/star_full.svg" alt="star icon">
      <img src="../../assets/icons/star_full.svg" alt="star icon">
      <img src="../../assets/icons/star_full.svg" alt="star icon">
      <img src="../../assets/icons/star_border.svg" alt="star icon">
    </div>
    <div class="flex justify-center">
      <button
        class="w-[114px] lg:h-[30px]  h-[20] text-xs lg:text-base border border-darkBlue rounded-md hover:bg-darkBlue hover:text-white">Lihat
        Detail</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      pakets: [
        { id: 1, jenis: "Medisline Paket 1", desc: "Lorem Ipsum is simply dummy text of the printing and typesetting industry.", img: "paket1.png" },
        { id: 2, jenis: "Medisline Paket 2", desc: "Lorem ipsum donor", img: "paket2.png" },
        { id: 3, jenis: "Medisline Paket 3", desc: "Lorem ipsum donor", img: "paket3.png" },
        { id: 4, jenis: "Medisline Paket 4", desc: "Lorem ipsum donor", img: "paket4.png" },
      ]
    }
  }
}
</script>

<style>
</style>