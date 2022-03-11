<template>
  <div class="member-details-container">
    <img :alt="image_alt" :src="image_src" class="member-details-image" />
    <h1 class="member-details-text textXL">{{ heading1 }}</h1>
    <h1 class="member-details-text1 textSM">{{ heading11 }}</h1>
  </div>
</template>

<script>
export default {
  name: 'MemberDetails',
  props: {
    heading11: {
      type: String,
      default: 'DEVELOPER/SYS ADMIN/CO-OWNER',
    },
    heading1: {
      type: String,
      default: 'Qemlokriu',
    },
    image_alt: {
      type: String,
      default: 'image',
    },
    image_src: {
      type: String,
      default: '385b2b93-d86f-4539-ba4b-3370a9b7c35f',
    },
  },
}
</script>

<style scoped>
.member-details-container {
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
}
.member-details-image {
  width: 100px;
  box-shadow: 0 10px 15px -3px rgba(0,0,0,0.1),0 4px 6px -2px rgba(0,0,0,0.05);
  object-fit: cover;
  border-radius: var(--dl-radius-radius-round);
}
.member-details-text {
  color: var(--dl-color-secondary-100);
  text-align: center;
  padding-top: var(--dl-space-space-unitandhalf);
}
.member-details-text1 {
  color: var(--dl-color-secondary-700);
  text-align: center;
  text-transform: uppercase;
}
</style>
