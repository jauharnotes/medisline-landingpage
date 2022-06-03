<template>
  <nav class="lg:mx-[81px] mx-2 pt-[9px] flex justify-between items-center">
    <div class="z-50">
      <img src="../../assets/images/logo-medisline.svg" alt="logo">
    </div>
    <div
      :class="toggle ? 'flex-col pt-14 text-center absolute top-0 w-full h-[600px] space-y-[50px] z-20 bg-white text-darkBlue' : 'lg:flex hidden space-x-2 md:space-x-[80px] text-darkBlue'">
      <a href="/" exact class="hover:text-[#01639C] hover:underline hover:underline-offset-8 cursor-pointer lg:inline-block block">Home</a>
      <a href="/service" class="hover:text-[#01639C] hover:underline hover:underline-offset-8 cursor-pointer lg:inline-block block">Service</a>
      <a href="/about" class="hover:text-[#01639C] hover:underline hover:underline-offset-8 cursor-pointer lg:inline-block block">About Us</a>
      <a href="/contact" class="hover:text-[#01639C] hover:underline hover:underline-offset-8 cursor-pointer lg:inline-block block">Contact Us</a>
    </div>
    <div
      :class="toggle ? 'space-x-[32px] absolute left-[50%] translate-x-[-50%] m-auto mt-[700px] z-40' : 'space-x-[32px] lg:flex hidden'">
      <button type="button"
        class="md:w-[104px] md:h-[32px] w-[89px] h-[27px] text-xs border-2 border-darkBlue rounded-full text-darkBlue hover:bg-[#01639C] hover:text-white">Register</button>
      <button type="button"
        class="md:w-[104px] md:h-[32px] w-[89px] h-[27px] text-xs border-2 rounded-full bg-darkBlue text-white hover:bg-[#01639C]">Login</button>
    </div>

    <!-- toggle menu -->

    <div @click="myFilter"
      :class="toggle ? 'lg:hidden flex-col active z-50 absolute top-2 right-2 cursor-pointer' : 'lg:hidden flex-col z-50 cursor-pointer'"
      id="navMenu">
      <span class="w-7 h-1 bg-darkBlue"></span>
      <span class="w-7 h-1 bg-darkBlue"></span>
      <span class="w-7 h-1 bg-darkBlue"></span>
    </div>

  </nav>
</template>

<script>
export default {
  data() {
    return {
      toggle: false
    }
  },
  methods: {
    myFilter: function () {
      this.toggle = !this.toggle;
    }
  }
}
</script>

<style>
#navMenu>span {
  display: block;
  width: 28px;
  height: 2px;
  border: none;
}

#navMenu>span:not(:last-child) {
  margin-bottom: 7px;
}

#navMenu,
#navMenu>span {
  transition: all .4s ease-in-out;
}

#navMenu.active {
  transition-delay: 0.8s;
  transform: rotate(45deg);
}

#navMenu.active>span:nth-child(2) {
  width: 0;
}

#navMenu.active>span:nth-child(1),
#navMenu.active>span:nth-child(3) {
  transition-delay: .4s;
}

#navMenu.active>span:nth-child(1) {
  transform: translateY(9px);
}

#navMenu.active>span:nth-child(3) {
  transform: translateY(-9px) rotate(90deg);
}
</style>