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
  data() {
    return {
      structuredData1: {
        '@context': 'http://schema.org',
        '@type': 'LocalBusiness',
        address: {
          '@type': 'PostalAddress',
          addressCountry: 'ES',
          addressLocality: 'Getafe',
          streetAddress: 'C/ Alcalde Angel Arroyo 10',
          postalCode: '28904',
        },
        description:
          'Consultoría y asesoramiento fiscal, contable, jurídico y laboral',
        name: 'Elite Asesor',
        telephone: '91 3304996',
      },
      structuredData2: {
        '@context': 'https://schema.org',
        '@type': ['LocalBusiness'],
        name: 'Elite Asesor',
        description:
          'Consultoría y asesoramiento fiscal, contable, jurídico y laboral',
        openingHours: [
          'Mo-Th 09:00-14:00',
          'Mo-Th 15:30-19:30',
          'Fr 09:00-15:00',
        ],
        currenciesAccepted: 'EUR',
        url: 'https://elite7.netlify.app/',
      },
    }
  },
  head() {
    return {
      script: [
        { type: 'application/ld+json', json: this.structuredData1 },
        { type: 'application/ld+json', json: this.structuredData2 },
      ],
    }
  },
}
</script>
