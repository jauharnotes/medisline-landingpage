<template>
  <div class="lg:mx-[81px] mx-2 pt-[9px] flex justify-between items-center">
    <div>
      <img src="../../assets/images/logo-medisline.svg" alt="logo">
    </div>
    <div
      :class="toggle ? 'flex-col pt-14 text-center absolute top-0 w-full h-[600px] space-y-[50px] z-20 bg-white text-darkBlue' : 'lg:flex hidden space-x-[80px] text-darkBlue'">
      <router-link to="/" exact class="hover:text-[#01639C] hover:underline hover:underline-offset-8 cursor-pointer">Home</router-link>
      <router-link to="/service" class="hover:text-[#01639C] hover:underline hover:underline-offset-8 cursor-pointer">Service</router-link>
      <router-link to="/about" class="hover:text-[#01639C] hover:underline hover:underline-offset-8 cursor-pointer">About Us</router-link>
      <router-link to="/contact" class="hover:text-[#01639C] hover:underline hover:underline-offset-8 cursor-pointer">Contact Us</router-link>
      <!-- <li><a href="#" class="hover:text-[#01639C] hover:underline hover:underline-offset-8">Service</a></li>
      <li><a href="#" class="hover:text-[#01639C] hover:underline hover:underline-offset-8">About Us</a></li>
      <li><a href="#" class="hover:text-[#01639C] hover:underline hover:underline-offset-8">Contact Us</a></li> -->
    </div>
    <div
      :class="toggle ? 'space-x-[32px] absolute left-[50%] translate-x-[-50%] m-auto mt-[700px] z-40' : 'space-x-[32px] lg:flex hidden'">
      <button type="button"
        class="w-[104px] h-[32px] text-xs border-2 border-darkBlue rounded-full text-darkBlue hover:bg-[#01639C] hover:text-white">Register</button>
      <button type="button"
        class="w-[104px] h-[32px] text-xs border-2 rounded-full bg-darkBlue text-white hover:bg-[#01639C]">Login</button>
    </div>

    <!-- toggle menu -->

    <button @click="myFilter"
      :class="toggle ? 'lg:hidden flex-col active z-50 absolute top-2 right-2' : 'lg:hidden flex-col z-50'"
      id="navMenu">
      <div class="w-7 h-1 bg-darkBlue"></div>
      <div class="w-7 h-1 bg-darkBlue"></div>
      <div class="w-7 h-1 bg-darkBlue"></div>
    </button>

  </div>
</template>

<script>
export default {
  data() {
    return {
      toggle: true
    }
  },
  methods: {
    myFilter: function () {
      this.toggle = !this.toggle;
      // some code to filter users
    }
  }
}
</script>

<style>
#navMenu>div {
  width: 28px;
  height: 2px;
}

#navMenu>div:not(:last-child) {
  margin-bottom: 7px;
}

#navMenu,
#navMenu>div {
  transition: all .4s ease-in-out;
}

#navMenu.active {
  transition-delay: 0.8s;
  transform: rotate(45deg);
}

#navMenu.active>div:nth-child(2) {
  width: 0;
}

#navMenu.active>div:nth-child(1),
#navMenu.active>div:nth-child(3) {
  transition-delay: .4s;
}

#navMenu.active>div:nth-child(1) {
  transform: translateY(9px);
}

#navMenu.active>div:nth-child(3) {
  transform: translateY(-9px) rotate(90deg);
}
</style>