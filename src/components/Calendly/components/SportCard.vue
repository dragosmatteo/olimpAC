<script>
export default {
  props: {
    title: String,
    text: String,
    imageSrc: String,
  },
};
</script>

<template>
  <app-card>
    <div class="image-overlay">
      <div class="content">
        <img
          :src="imageSrc"
          class="h-[664px] smd:h-[664px] xl:h-auto w-full"
          alt="football"
        />

        <div class="content-details fadeIn-bottom fadeIn-right">
          <div class="content-text">
            <h4>{{ title }}</h4>
            <p>
              {{ text }}
            </p>
          </div>
          <a href="#">
            <button
              class="content-button mt-[16px] flex font-rubik text-[#E9C65C] text-[14px] items-center px-[35px] py-[15px] font-semibold justify-center gap-[10px] rounded-full border-2 border-[#E9C65C] bg-transparent focus:outline-none transition duration-300 hover:bg-[#E9C65C] hover:text-black"
            >
              INSCRIE-TE ACUM!
            </button>
          </a>
        </div>
      </div>
    </div>

    <div class="mt-[16px]">
      <div class="flex flex-row justify-left items-center gap-[32px]">
        <h4
          class="text-white font-syne text-[24px] font-bold leading-[133.333%]"
        >
          Football - 29 Mai
        </h4>

        <div class="w-[48px] h-px bg-[#213B2A]"></div>
      </div>

      <div class="mt-[32px] flex gap-7">
        <p
          class="text-silver font-rubik text-base font-normal leading-[137.5%] tracking-tighter"
        >
          Ora:
        </p>
        <span
          class="text-white font-Rubik text-base font-normal leading-[137.5%] tracking-[0.25px]"
          >15:00</span
        >
      </div>
      <div class="flex gap-4">
        <p
          class="text-silver font-rubik text-base font-normal leading-[137.5%] tracking-tighter"
        >
          Unde:
        </p>
        <span
          class="text-white font-Rubik text-base font-normal leading-[137.5%] tracking-[0.25px]"
          >Teren Fotbal 1 Teren Fotbal 1</span
        >
      </div>
    </div>
  </app-card>
</template>

<style>
.content {
  position: relative;
  overflow: hidden;
  cursor: pointer;
}

.content .content-overlay {
  position: absolute;
  height: 100%;
  width: 100%;
  -webkit-transition: all 0.4s ease-in-out 0s;
  -moz-transition: all 0.4s ease-in-out 0s;
  transition: all 0.4s ease-in-out 0s;
}

.content-details {
  font-family: "Syne", sans-serif;
  position: absolute;
  text-align: left;
  padding-left: 1em;
  padding-right: 1em;
  width: 100%;
  height: 100%;
  top: 50%;
  left: 50%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
  -webkit-transform: translate(-50%, -50%);
  -moz-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  -webkit-transition: all 0.3s ease-in-out 0s;
  -moz-transition: all 0.3s ease-in-out 0s;
  transition: all 0.3s ease-in-out 0s;
  border-radius: 16px;
}

.content-details::before {
  content: " ";
  width: 20px;
  height: 20px;
  position: absolute;
  background: rgba(0, 0, 0, 0.7);
  bottom: -20px;
  right: -20px;
  border-radius: 50%;
  transition: height 0.3s ease-in-out, width 0.3s ease-in-out, border-radius 0.05s ease-in-out;
}

.content:hover .content-details::before {
  height: 100%;
  width: 100%;
  border-radius: 16px;
  bottom: 0;
  right: 0;
}

.content:hover .content-details {
  display: flex;
}

.content:hover .content-text {
  transform: translate(0, 0);
}

.content:hover .content-button {
  transform: translate(0, 0);
}

.content-details h4 {
  color: #fff;
  font-family: Syne;
  font-size: 24px;
  font-style: normal;
  font-weight: 700;
  line-height: 18px; /* 90% */
  letter-spacing: 0.25px;
}

.content-text {
  transform: translate(0, -200%);
  transition: all ease-in-out 0.5s;
}

.content-button {
  transform: translate(-200%, 0);
  transition: all ease-in-out 0.5s;
}

.content-details p {
  margin-top: 16px;
  font-size: 16px;
  color: #bebfc4;
  font-family: "Rubik", sans-serif;
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 18px;
  letter-spacing: 0.25px;
}

.image-overlay {
  overflow: hidden;
}
</style>
