<template>
  <div class="font-fontAlt mt-[72px] text-blue relative mb-[199px] text-center">
    <div class="flex flex-col items-center justify-center space-y-4">
      <h2 class="font-bold text-4xl lg:text-5xl">{{ title }}</h2>
      <p class="text-[32px]">{{ desc }}</p>
    </div>
    <div class="flex flex-wrap justify-center gap-20 mt-[88px]">
      <div v-for="(card, index) in cards" :key="card.id">
        <div
          :class="index === 1 ? 'flex justify-center items-center scale-125 w-[300px] h-[380px] shadow-md bg-white rounded-2xl transition ease-in-out duration-150 hover:bg-blue hover:text-white group' : 'flex justify-center items-center w-[300px] h-[380px] shadow-md bg-white rounded-2xl transition ease-in-out duration-150 hover:bg-blue hover:text-white group'">
          <div class="flex items-center justify-center">
            <div class="flex-col space-y-7 px-8">
              <h2 class="font-bold text-lg underline underline-offset-4 text-center">{{ card.name }}</h2>
              <div class="flex justify-end -mr-3">
                <svg width="30" height="23" viewBox="0 0 30 23" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path
                    d="M18.8439 10.2969L18.8439 0.5H30V8.23438C30 12.4219 29.3834 15.4531 28.1503 17.3281C26.5318 19.8281 23.9692 21.7187 20.4624 23L17.9191 19.7187C20.0385 19 21.5992 17.9219 22.6012 16.4844C23.6031 15.0781 24.1618 13.0156 24.2775 10.2969L18.8439 10.2969ZM0.924855 10.2969L0.924855 0.5H12.0809V8.23438C12.0809 12.4219 11.4644 15.4531 10.2312 17.3281C8.61272 19.8281 6.05009 21.7187 2.54335 23L-7.15256e-07 19.7187C2.11946 19 3.68015 17.9219 4.68208 16.4844C5.68401 15.0781 6.24277 13.0156 6.35838 10.2969H0.924855Z"
                    class="fill-[#0C467E] group-hover:fill-white" />
                </svg>
              </div>
              <p class="text-center text-xs">{{ card.desc }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="absolute w-full -bottom-72 -z-20">
      <img class="w-full" src="../../assets/images/bg-circle.png" alt="">
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      scale: false,
      title: "92% pasien Medisline merasa lebih baik",
      desc: "Pasien Medisline telah merasakan pelayanan yang optimal oleh tenaga profesional ",
      cards: [
        { id: 1, name: "Nama Pasien", desc: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book." },
        { id: 2, name: "Nama Pasien", desc: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book." },
        { id: 3, name: "Nama Pasien", desc: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book." },
      ]
    }
  },
  methods: {
    scale() {
      this.scale.classList.add("my-class");
    }
  }
}
</script>
