<template>
  <div>
    <!-- This example requires Tailwind CSS v2.0+ -->
    <div class="bg-red-50">
      <div class="container">
        <div
          class="max-w-7xl mx-auto py-12 px-4 sm:px-6 lg:py-24 lg:px-8 lg:flex lg:items-center lg:justify-between"
        >
          <h2
            class="text-3xl font-extrabold tracking-tight text-gray-900 md:text-4xl"
          >
            <span class="block">Consultores y asesores.</span>
            <span class="block text-red-600">Estamos aquí para ayudarte.</span>
          </h2>
          <div class="mt-8 flex lg:mt-0 lg:flex-shrink-0">
            <div class="flex rounded-md shadow">
              <nuxt-link
                to="contacto"
                target="_blank"
                class="inline-flex items-center justify-center px-5 py-3 border border-transparent text-base font-bold rounded-md text-white bg-red-600 hover:bg-red-700"
              >
                Quiero asesoramiento
              </nuxt-link>
            </div>
          </div>
        </div>
      </div>
    </div>

    <section>
      <!-- This example requires Tailwind CSS v2.0+ -->
      <div class="py-16 bg-gray-50 overflow-hidden lg:py-24">
        <div
          class="relative max-w-xl mx-auto px-4 sm:px-6 lg:px-8 lg:max-w-7xl"
        >
          <svg
            class="hidden lg:block absolute left-full transform -translate-x-1/2 -translate-y-1/4"
            width="404"
            height="784"
            fill="none"
            viewBox="0 0 404 784"
            aria-hidden="true"
          >
            <defs>
              <pattern
                id="b1e6e422-73f8-40a6-b5d9-c8586e37e0e7"
                x="0"
                y="0"
                width="20"
                height="20"
                patternUnits="userSpaceOnUse"
              >
                <rect
                  x="0"
                  y="0"
                  width="4"
                  height="4"
                  class="text-gray-200"
                  fill="currentColor"
                />
              </pattern>
            </defs>
            <rect
              width="404"
              height="784"
              fill="url(#b1e6e422-73f8-40a6-b5d9-c8586e37e0e7)"
            />
          </svg>

          <div class="relative">
            <h2
              class="text-center text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl"
            >
              Haz crecer tu negocio
            </h2>
            <p class="mt-4 max-w-3xl mx-auto text-center text-xl text-gray-500">
              Consultoría y asesoría de élite. Ahorra tiempo en la gestión de tu
              negocio. Evita errores y sanciones de Hacienda.
            </p>
          </div>

          <div
            class="relative mt-12 lg:mt-24 lg:grid lg:grid-cols-2 lg:gap-8 lg:items-center"
          >
            <div class="relative">
              <h3
                class="text-2xl font-extrabold text-gray-900 tracking-tight sm:text-3xl"
              >
                Asesores y consultores
              </h3>
              <p class="mt-3 text-lg text-gray-500">
                Te asesoramos y acompañamos en lo que necesites para hacer
                crecer tu negocio.
              </p>

              <dl class="mt-10 space-y-10">
                <div class="relative">
                  <dt>
                    <div
                      class="absolute flex items-center justify-center h-12 w-12 rounded-md bg-red-500 text-white"
                    >
                      <svg-fiscal></svg-fiscal>
                    </div>
                    <p
                      class="ml-16 text-lg leading-6 font-medium text-gray-900"
                    >
                      Asesoramiento Fiscal
                    </p>
                  </dt>
                  <dd class="mt-2 ml-16 text-base text-gray-500">
                    Asesoramiento en todo tipo de materia tributaria a empresas,
                    autónomos y particulares.
                    <ul class="pt-2">
                      <li
                        v-for="(item, idx) in fiscalItems"
                        :key="`item-${idx}`"
                        class="pb-2 flex"
                      >
                        <svg
                          class="flex-shrink-0 h-6 w-6 text-green-500"
                          xmlns="http://www.w3.org/2000/svg"
                          fill="none"
                          viewBox="0 0 24 24"
                          stroke="currentColor"
                          aria-hidden="true"
                        >
                          <path
                            stroke-linecap="round"
                            stroke-linejoin="round"
                            stroke-width="2"
                            d="M5 13l4 4L19 7"
                          />
                        </svg>
                        <span class="ml-3 text-base text-gray-500">
                          {{ item }}
                        </span>
                      </li>
                    </ul>
                  </dd>
                </div>

                <div class="relative">
                  <dt>
                    <div
                      class="absolute flex items-center justify-center h-12 w-12 rounded-md bg-red-500 text-white"
                    >
                      <svg-contable></svg-contable>
                    </div>
                    <p
                      class="ml-16 text-lg leading-6 font-medium text-gray-900"
                    >
                      Asesoramiento Contable
                    </p>
                  </dt>
                  <dd class="mt-2 ml-16 text-base text-gray-500">
                    Asesoramiento contable y concepción de contabilidades a
                    entidades mercantiles y autónomos.

                    <ul class="pt-2">
                      <li
                        v-for="(item, idx) in contableItems"
                        :key="`item-${idx}`"
                        class="pb-2 flex"
                      >
                        <svg
                          class="flex-shrink-0 h-6 w-6 text-green-500"
                          xmlns="http://www.w3.org/2000/svg"
                          fill="none"
                          viewBox="0 0 24 24"
                          stroke="currentColor"
                          aria-hidden="true"
                        >
                          <path
                            stroke-linecap="round"
                            stroke-linejoin="round"
                            stroke-width="2"
                            d="M5 13l4 4L19 7"
                          />
                        </svg>
                        <span class="ml-3 text-base text-gray-500">
                          {{ item }}
                        </span>
                      </li>
                    </ul>
                  </dd>
                </div>
              </dl>
            </div>

            <div class="mt-10 -mx-4 relative lg:mt-0" aria-hidden="true">
              <svg
                class="absolute left-1/2 transform -translate-x-1/2 translate-y-16 lg:hidden"
                width="784"
                height="404"
                fill="none"
                viewBox="0 0 784 404"
              >
                <defs>
                  <pattern
                    id="ca9667ae-9f92-4be7-abcb-9e3d727f2941"
                    x="0"
                    y="0"
                    width="20"
                    height="20"
                    patternUnits="userSpaceOnUse"
                  >
                    <rect
                      x="0"
                      y="0"
                      width="4"
                      height="4"
                      class="text-gray-200"
                      fill="currentColor"
                    />
                  </pattern>
                </defs>
                <rect
                  width="784"
                  height="404"
                  fill="url(#ca9667ae-9f92-4be7-abcb-9e3d727f2941)"
                />
              </svg>
              <img
                class="relative mx-auto"
                width="490"
                src="/servicios/spreadsheet.svg"
                alt="ilustración hoja de excel"
              />
            </div>
          </div>

          <svg
            class="hidden lg:block absolute right-full transform translate-x-1/2 translate-y-12"
            width="404"
            height="784"
            fill="none"
            viewBox="0 0 404 784"
            aria-hidden="true"
          >
            <defs>
              <pattern
                id="64e643ad-2176-4f86-b3d7-f2c5da3b6a6d"
                x="0"
                y="0"
                width="20"
                height="20"
                patternUnits="userSpaceOnUse"
              >
                <rect
                  x="0"
                  y="0"
                  width="4"
                  height="4"
                  class="text-gray-200"
                  fill="currentColor"
                />
              </pattern>
            </defs>
            <rect
              width="404"
              height="784"
              fill="url(#64e643ad-2176-4f86-b3d7-f2c5da3b6a6d)"
            />
          </svg>

          <div class="relative mt-12 sm:mt-16 lg:mt-24">
            <div
              class="lg:grid lg:grid-flow-row-dense lg:grid-cols-2 lg:gap-8 lg:items-center"
            >
              <div class="lg:col-start-2">
                <h3
                  class="text-2xl font-extrabold text-gray-900 tracking-tight sm:text-3xl"
                >
                  Particulares o Empresas
                </h3>
                <p class="mt-3 text-lg text-gray-500">
                  Resolvemos sus problemas, minimizamos sus riesgos y le
                  ahorramos tiempo y recursos. ¡Llama ya!
                </p>

                <dl class="mt-10 space-y-10">
                  <div class="relative">
                    <dt>
                      <div
                        class="absolute flex items-center justify-center h-12 w-12 rounded-md bg-red-500 text-white"
                      >
                        <svg-juridico></svg-juridico>
                      </div>
                      <p
                        class="ml-16 text-lg leading-6 font-medium text-gray-900"
                      >
                        Asesoramiento Jurídico
                      </p>
                    </dt>
                    <dd class="mt-2 ml-16 text-base text-gray-500">
                      Asesoramiento en derecho mercantil, tributario y laboral.
                      Derecho civil, penal y administrativo.

                      <ul class="pt-2">
                        <li
                          v-for="(item, idx) in juridicoItems"
                          :key="`item-${idx}`"
                          class="pb-2 flex"
                        >
                          <svg
                            class="flex-shrink-0 h-6 w-6 text-green-500"
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            stroke="currentColor"
                            aria-hidden="true"
                          >
                            <path
                              stroke-linecap="round"
                              stroke-linejoin="round"
                              stroke-width="2"
                              d="M5 13l4 4L19 7"
                            />
                          </svg>
                          <span class="ml-3 text-base text-gray-500">
                            {{ item }}
                          </span>
                        </li>
                      </ul>
                    </dd>
                  </div>

                  <div class="relative">
                    <dt>
                      <div
                        class="absolute flex items-center justify-center h-12 w-12 rounded-md bg-red-500 text-white"
                      >
                        <svg-laboral></svg-laboral>
                      </div>
                      <p
                        class="ml-16 text-lg leading-6 font-medium text-gray-900"
                      >
                        Asesoramiento Laboral
                      </p>
                    </dt>
                    <dd class="mt-2 ml-16 text-base text-gray-500">
                      Elaboración de nóminas, seguros sociales, impuestos.
                      Altas, bajas, modificaciones en seguridad social.

                      <ul class="pt-2">
                        <li
                          v-for="(item, idx) in laboralItems"
                          :key="`item-${idx}`"
                          class="pb-2 flex"
                        >
                          <svg
                            class="flex-shrink-0 h-6 w-6 text-green-500"
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            stroke="currentColor"
                            aria-hidden="true"
                          >
                            <path
                              stroke-linecap="round"
                              stroke-linejoin="round"
                              stroke-width="2"
                              d="M5 13l4 4L19 7"
                            />
                          </svg>
                          <span class="ml-3 text-base text-gray-500">
                            {{ item }}
                          </span>
                        </li>
                      </ul>
                    </dd>
                  </div>
                </dl>
              </div>

              <div class="mt-10 -mx-4 relative lg:mt-0 lg:col-start-1">
                <svg
                  class="absolute left-1/2 transform -translate-x-1/2 translate-y-16 lg:hidden"
                  width="784"
                  height="404"
                  fill="none"
                  viewBox="0 0 784 404"
                  aria-hidden="true"
                >
                  <defs>
                    <pattern
                      id="e80155a9-dfde-425a-b5ea-1f6fadd20131"
                      x="0"
                      y="0"
                      width="20"
                      height="20"
                      patternUnits="userSpaceOnUse"
                    >
                      <rect
                        x="0"
                        y="0"
                        width="4"
                        height="4"
                        class="text-gray-200"
                        fill="currentColor"
                      />
                    </pattern>
                  </defs>
                  <rect
                    width="784"
                    height="404"
                    fill="url(#e80155a9-dfde-425a-b5ea-1f6fadd20131)"
                  />
                </svg>
                <img
                  class="relative mx-auto"
                  width="490"
                  src="/servicios/agreement.svg"
                  alt="ilustración contrato"
                />
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import {
  SvgLaboral,
  SvgContable,
  SvgJuridico,
  SvgFiscal,
} from '~/components/svgIcons/index.js'

export default {
  name: 'Servicios',
  components: { SvgLaboral, SvgContable, SvgJuridico, SvgFiscal },
  data() {
    return {
      fiscalItems: [
        'Asesoramiento en materia tributaria a empresas, autónomos y particulares.',
        'Concepcion, revision y presentación de todo tipo de impuestos. ',
        'Asesoramiento y planificación de inspecciones tributarias',
      ],
      contableItems: [
        'Asesoramiento y concepción de contabilidades a entidades mercantiles y autónomos.',
        'Información de novedades en materia contable.',
        'Preparación y presentación de cuentas anuales.',
        'Análisis de balance.',
      ],
      laboralItems: [
        'Asesoramiento en materia de seguridad social.',
        'Elaboración de nominas, seguros sociales, impuestos.',
        'Altas, bajas,  modificaciones en seguridad social.',
        'ERTEs, EREs.',
        'Despidos.',
      ],
      juridicoItems: [
        'Asesoramiento en derecho mercantil, tributario y laboral.',
        'Derecho civil, penal y administrativo.',
        'Concurso de acreedores, ',
        'Herencias',
        'Reclamaciones de cantidad',
      ],
    }
  },
}
</script>
