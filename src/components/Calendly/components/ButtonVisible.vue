<template>
  <app-card>
    <div class="full-details-button inline-flex sm:hidden" @click="toggleContent">Click to read more</div>
  </app-card>
</template>

<style>
.full-details-button{
    background: #BEBFC4;
    font-size: 16px;
    padding: 12px 24px;
    font-weight: 500;
    position: absolute;
    z-index: 4;
    bottom: 0;
    right: 0;
    border-radius: 16px 0px 16px 0px;
    color: #060E0F;

}
</style>

<script>
export default {
  methods: {
    toggleContent() {
      this.$emit('toggle-content');
    }
  }
}
</script>