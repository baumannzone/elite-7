<template>
  <div>
    <HeaderSection />

    <ServicesSection />

    <MoreServicesSection />
  </div>
</template>

<script>
import HeaderSection from '~/components/home/HeaderSection'
import ServicesSection from '~/components/home/ServicesSection'
import MoreServicesSection from '~/components/home/MoreServicesSection'

export default {
  components: { MoreServicesSection, ServicesSection, HeaderSection },
}
</script>
