<template>
  <div class="w-full h-[459px] bg-sliteBlue mt-4 flex flex-col justify-center items-center md:text-left pl-9 text-center">
    <div class="lg:mx-[81px] lg:flex  justify-around gap-20">
      <div class="md:flex-1 flex-col max-w-[489px] space-y-2 text-darkBlue">
        <div v-html="heading"></div>
        <p>{{ desc }}</p>
      </div>
      <div class="lg:flex-1 w-full  md:inline-block">
        <img src="../../assets/images/doctor.png" alt="doctor" width="505.35">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      heading:
        '<h2 class="font-bold w-full text-4xl lg:text-5xl lg:leading-normal mt-6">Selamat Datang <br> Di Layanan Medisline</h2>',
      desc: 'Kami adalah Layanan Kesehatan Masyarakat Berbasis Website yang siap melayani Indonesia',
    };
  },
};
</script>
