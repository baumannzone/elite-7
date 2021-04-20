<template>
  <div>
    <HeaderSection />

    <ServicesSection />

    <ContactSection />
  </div>
</template>

<script>
import HeaderSection from '~/components/home/HeaderSection'
import ServicesSection from '~/components/home/ServicesSection'
import ContactSection from '~/components/home/ContactSection'

export default {
  components: {
    HeaderSection,
    ServicesSection,
    ContactSection,
  },
}
</script>
