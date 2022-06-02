<template>
  <div class="flex flex-wrap gap-10 justify-between pt-[86px] px-[70px] bg-[#00264A] w-full h-full lg:h-[462px] pb-6">
    <div class="flex flex-col items-start">
      <h2 class="font-bold text-4xl text-[#85C2FC]">Medisline</h2>
      <p class="font-light max-w-[390px] text-white mt-4">Lorem Ipsum is simply dummy text of the printing and
        typesetting industry. Lorem Ipsum has been the industry's standard dummy text.</p>
      <div class="flex items-center gap-4 my-[40px]">
        <img src="../../assets/icons/phone-call.svg" alt="facebook icon">
        <h1 class="text-white text-lg">BUTUH BANTUAN <br> 021-555-721 / 081328000555</h1>
      </div>
      <div class="flex gap-4">
        <a href=""><img src="../../assets/icons/facebook.svg" width="40" alt="facebook icon"
            class="hover:scale-105"></a>
        <a href=""><img src="../../assets/icons/twitter.svg" width="40" alt="twitter icon" class="hover:scale-105"></a>
        <a href=""><img src="../../assets/icons/instagram.svg" width="40" alt="instagram icon"
            class="hover:scale-105"></a>
        <a href=""><img src="../../assets/icons/linkedin.svg" width="40" alt="linkedin icon"
            class="hover:scale-105"></a>
      </div>
    </div>
    <div class="flex flex-col items-start">
      <ul class="text-white text-base space-y-4">
        <li><a href="" class="hover:underline hover:underline-offset-4">Tentang Kami</a></li>
        <li><a href="" class="hover:underline hover:underline-offset-4">Pertanyaan</a></li>
        <li><a href="" class="hover:underline hover:underline-offset-4">Kebijakan Privasi</a></li>
        <li><a href="" class="hover:underline hover:underline-offset-4">Kesepakatan Layanan</a></li>
        <li><a href="" class="hover:underline hover:underline-offset-4">Kontak Kami</a></li>
        <li><a href="" class="hover:underline hover:underline-offset-4">Karir</a></li>
      </ul>
    </div>
    <div class="flex flex-col gap-4 items-start max-w-[405px]">
      <p class="text-sm text-white">You may unsubscribe at any moment. For that purpose, please find our contact info in
        the legal notice.</p>
      <div class="space-x-3 space-y-4">
        <input type="email" placeholder="Your email address" class="w-[271px] h-[40px] rounded-full bg-white px-4 placeholder-[#85C2FC] placeholder-opacity-50 focus:outline-none focus:border-sky-500 focus:ring-1 focus:ring-sky-500
      disabled:bg-slate-50 disabled:text-slate-500 disabled:border-slate-200 disabled:shadow-none
      invalid:border-pink-500 invalid:text-pink-600
      focus:invalid:border-pink-500 focus:invalid:ring-pink-500">
        <button class="w-[106px] h-[40px] text-white bg-[#85C2FC] rounded-full hover:bg-darkBlue">subscribe</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>
