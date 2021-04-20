<template>
  <div>
    <!-- This example requires Tailwind CSS v2.0+ -->
    <div class="min-h-screen bg-white">
      <main>
        <div class="mt-16">
          <!-- Hero card -->
          <div class="relative">
            <div class="absolute inset-x-0 bottom-0 h-1/2 bg-gray-100"></div>
            <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
              <div class="relative shadow-xl sm:rounded-2xl sm:overflow-hidden">
                <div class="absolute inset-0">
                  <img
                    class="h-full w-full object-cover"
                    src="https://images.unsplash.com/photo-1521737852567-6949f3f9f2b5?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=2830&q=80&sat=-100"
                    alt="People working on laptops"
                  />
                  <div
                    class="absolute inset-0 bg-indigo-700"
                    style="mix-blend-mode: multiply"
                  ></div>
                </div>
                <div
                  class="relative px-4 py-16 sm:px-6 sm:py-24 lg:py-32 lg:px-8"
                >
                  <h1
                    class="text-center text-4xl font-extrabold tracking-tight sm:text-5xl lg:text-6xl"
                  >
                    <span class="block text-white">Take control of your</span>
                    <span class="block text-indigo-200">customer support</span>
                  </h1>
                  <p
                    class="mt-6 max-w-lg mx-auto text-center text-xl text-indigo-200 sm:max-w-3xl"
                  >
                    Anim aute id magna aliqua ad ad non deserunt sunt. Qui irure
                    qui lorem cupidatat commodo. Elit sunt amet fugiat veniam
                    occaecat fugiat aliqua.
                  </p>
                  <div
                    class="mt-10 max-w-sm mx-auto sm:max-w-none sm:flex sm:justify-center"
                  >
                    <div
                      class="space-y-4 sm:space-y-0 sm:mx-auto sm:inline-grid sm:grid-cols-2 sm:gap-5"
                    >
                      <a
                        href="#"
                        class="flex items-center justify-center px-4 py-3 border border-transparent text-base font-medium rounded-md shadow-sm text-indigo-700 bg-white hover:bg-indigo-50 sm:px-8"
                      >
                        Get started
                      </a>
                      <a
                        href="#"
                        class="flex items-center justify-center px-4 py-3 border border-transparent text-base font-medium rounded-md shadow-sm text-white bg-indigo-500 bg-opacity-60 hover:bg-opacity-70 sm:px-8"
                      >
                        Live demo
                      </a>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <!-- Logo cloud -->
          <div class="bg-gray-100">
            <div class="max-w-7xl mx-auto py-16 px-4 sm:px-6 lg:px-8">
              <p
                class="text-center text-sm font-semibold uppercase text-gray-500 tracking-wide"
              >
                Trusted by over 5 very average small businesses
              </p>
              <div
                class="mt-6 grid grid-cols-2 gap-8 md:grid-cols-6 lg:grid-cols-5"
              >
                <div
                  class="col-span-1 flex justify-center md:col-span-2 lg:col-span-1"
                >
                  <img
                    class="h-12"
                    src="https://tailwindui.com/img/logos/tuple-logo-gray-400.svg"
                    alt="Tuple"
                  />
                </div>
                <div
                  class="col-span-1 flex justify-center md:col-span-2 lg:col-span-1"
                >
                  <img
                    class="h-12"
                    src="https://tailwindui.com/img/logos/mirage-logo-gray-400.svg"
                    alt="Mirage"
                  />
                </div>
                <div
                  class="col-span-1 flex justify-center md:col-span-2 lg:col-span-1"
                >
                  <img
                    class="h-12"
                    src="https://tailwindui.com/img/logos/statickit-logo-gray-400.svg"
                    alt="StaticKit"
                  />
                </div>
                <div
                  class="col-span-1 flex justify-center md:col-span-2 md:col-start-2 lg:col-span-1"
                >
                  <img
                    class="h-12"
                    src="https://tailwindui.com/img/logos/transistor-logo-gray-400.svg"
                    alt="Transistor"
                  />
                </div>
                <div
                  class="col-span-2 flex justify-center md:col-span-2 md:col-start-4 lg:col-span-1"
                >
                  <img
                    class="h-12"
                    src="https://tailwindui.com/img/logos/workcation-logo-gray-400.svg"
                    alt="Workcation"
                  />
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- More main page content here... -->
      </main>
    </div>

    <div class="container">
      <section>
        <!-- This example requires Tailwind CSS v2.0+ -->
        <div class="py-12 bg-white">
          <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="lg:text-center">
              <h2
                class="text-base text-red-600 font-semibold tracking-wide uppercase"
              >
                Nuestros servicios
              </h2>
              <p
                class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl"
              >
                Consultoría y asesoramiento
              </p>
              <p class="mt-4 max-w-2xl text-xl text-gray-500 lg:mx-auto">
                Prestamos servicios de consultoría y asesoramiento fiscal,
                contable, jurídico y laboral a particulares y empresas.
              </p>
            </div>

            <div class="mt-10">
              <dl
                class="space-y-10 md:space-y-0 md:grid md:grid-cols-2 md:gap-x-8 md:gap-y-10"
              >
                <div class="flex">
                  <div class="flex-shrink-0">
                    <div
                      class="flex items-center justify-center h-12 w-12 rounded-md bg-red-500 text-white"
                    >
                      <!-- Heroicon name: lightning-bolt -->
                      <svg
                        class="h-6 w-6"
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
                          d="M13 10V3L4 14h7v7l9-11h-7z"
                        />
                      </svg>
                    </div>
                  </div>
                  <div class="ml-4">
                    <dt class="text-lg leading-6 font-medium text-gray-900">
                      Asesoramiento Fiscal
                    </dt>
                    <dd class="mt-2 text-base text-gray-500">
                      Asesoramiento en todo tipo de materia tributaria a
                      empresas, autónomos y particulares.
                    </dd>
                  </div>
                </div>

                <div class="flex">
                  <div class="flex-shrink-0">
                    <div
                      class="flex items-center justify-center h-12 w-12 rounded-md bg-red-500 text-white"
                    >
                      <!-- Heroicon name: annotation -->
                      <svg
                        class="h-6 w-6"
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
                          d="M7 8h10M7 12h4m1 8l-4-4H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-3l-4 4z"
                        />
                      </svg>
                    </div>
                  </div>
                  <div class="ml-4">
                    <dt class="text-lg leading-6 font-medium text-gray-900">
                      Asesoramiento Contable
                    </dt>
                    <dd class="mt-2 text-base text-gray-500">
                      Asesoramiento contable y concepción de contabilidades a
                      entidades mercantiles y autónomos.
                    </dd>
                  </div>
                </div>

                <div class="flex">
                  <div class="flex-shrink-0">
                    <div
                      class="flex items-center justify-center h-12 w-12 rounded-md bg-red-500 text-white"
                    >
                      <!-- Heroicon name: globe-alt -->
                      <svg
                        class="h-6 w-6"
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
                          d="M21 12a9 9 0 01-9 9m9-9a9 9 0 00-9-9m9 9H3m9 9a9 9 0 01-9-9m9 9c1.657 0 3-4.03 3-9s-1.343-9-3-9m0 18c-1.657 0-3-4.03-3-9s1.343-9 3-9m-9 9a9 9 0 019-9"
                        />
                      </svg>
                    </div>
                  </div>
                  <div class="ml-4">
                    <dt class="text-lg leading-6 font-medium text-gray-900">
                      Asesoramiento Jurídico
                    </dt>
                    <dd class="mt-2 text-base text-gray-500">
                      Asesoramiento en derecho mercantil, tributario y laboral.
                      Derecho civil, penal y administrativo.
                    </dd>
                  </div>
                </div>

                <div class="flex">
                  <div class="flex-shrink-0">
                    <div
                      class="flex items-center justify-center h-12 w-12 rounded-md bg-red-500 text-white"
                    >
                      <!-- Heroicon name: scale -->
                      <svg
                        class="h-6 w-6"
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
                          d="M3 6l3 1m0 0l-3 9a5.002 5.002 0 006.001 0M6 7l3 9M6 7l6-2m6 2l3-1m-3 1l-3 9a5.002 5.002 0 006.001 0M18 7l3 9m-3-9l-6-2m0-2v2m0 16V5m0 16H9m3 0h3"
                        />
                      </svg>
                    </div>
                  </div>
                  <div class="ml-4">
                    <dt class="text-lg leading-6 font-medium text-gray-900">
                      Asesoramiento Laboral
                    </dt>
                    <dd class="mt-2 text-base text-gray-500">
                      Elaboración de nóminas, seguros sociales, impuestos.
                      Altas, bajas, modificaciones en seguridad social.
                    </dd>
                  </div>
                </div>
              </dl>
            </div>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
export default {}
</script>
