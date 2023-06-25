<template>
  <!-- navbar -->
  <section>
    <header class="bg-white">
      <nav
        class="mx-auto flex max-w-7xl items-center justify-between p-6 lg:px-8"
        aria-label="Global"
      >
        <div class="flex lg:flex-1">
          <a href="#" class="-m-1.5 p-1.5">
            <img
              class="h-8 w-auto"
              src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=600"
              alt=""
            />
          </a>
        </div>
        <div class="flex lg:hidden">
          <button
            type="button"
            class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-700"
            @click="mobileMenuOpen = true"
          >
            <span class="sr-only">Open main menu</span>
            <Bars3Icon class="h-6 w-6" aria-hidden="true" />
          </button>
        </div>
        <PopoverGroup class="hidden lg:flex lg:gap-x-12">
          <a href="#" class="text-sm font-semibold leading-6 text-gray-900"
            >Produit</a
          >

          <a href="#" class="text-sm font-semibold leading-6 text-gray-900"
            >Solutions</a
          >
          <a href="#" class="text-sm font-semibold leading-6 text-gray-900"
            >Contact</a
          >
          <a href="#" class="text-sm font-semibold leading-6 text-gray-900"
            >FAQ</a
          >
        </PopoverGroup>
        <div class="hidden lg:flex lg:flex-1 lg:justify-end">
          <!-- <a href="#" class="text-sm font-semibold leading-6 text-gray-900"
            >Log in <span aria-hidden="true">&rarr;</span></a
          > -->
        </div>
      </nav>
      <Dialog
        as="div"
        class="lg:hidden"
        @close="mobileMenuOpen = false"
        :open="mobileMenuOpen"
      >
        <div class="fixed inset-0 z-10" />
        <DialogPanel
          class="fixed inset-y-0 right-0 z-10 w-full overflow-y-auto bg-white px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-gray-900/10"
        >
          <div class="flex items-center justify-between">
            <a href="#" class="-m-1.5 p-1.5">
              <img
                class="h-8 w-auto"
                src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=600"
                alt=""
              />
            </a>
            <button
              type="button"
              class="-m-2.5 rounded-md p-2.5 text-gray-700"
              @click="mobileMenuOpen = false"
            >
              <span class="sr-only">Close menu</span>
              <XMarkIcon class="h-6 w-6" aria-hidden="true" />
            </button>
          </div>
          <div class="mt-6 flow-root">
            <div class="-my-6 divide-y divide-gray-500/10">
              <div class="space-y-2 py-6">
                <a
                  href="#"
                  class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-50"
                >
                  Produit
                </a>
                <a
                  href="#"
                  class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-50"
                  >Solutions</a
                >
                <a
                  href="#"
                  class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-50"
                  >Contact</a
                >
                <a
                  href="#"
                  class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-50"
                  >FAQ</a
                >
              </div>
              <div class="py-6">
                <!-- <a
                  href="#"
                  class="-mx-3 block rounded-lg px-3 py-2.5 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-50"
                  >Log in</a
                > -->
              </div>
            </div>
          </div>
        </DialogPanel>
      </Dialog>
    </header>
  </section>
  <!-- hero -->
  <section class="bg-white dark:bg-gray-900">
    <div class="grid lg:mt-0 lg:grid-cols-12">
      <div class="py-32 max-w-screen-xl text-center lg:col-span-7">
        <h1
          class="mb-4 text-4xl font-extrabold tracking-tight leading-none text-gray-900 md:text-5xl lg:text-6xl dark:text-white"
        >
          <span style="color: #7e22ce"> ScanEat</span> une expérience unique de
          commande pour votre restaurant.
          <!-- Révolutionnez l'expérience de commande de votre restaurant -->
        </h1>
        <p
          class="mb-8 text-lg font-normal text-gray-500 lg:text-xl sm:px-4 xl:px-4 dark:text-gray-400"
        >
          Une interface conviviale, des menus interactifs et des options de
          personnalisation <br />
          avancées, le tout à portée de main.
        </p>
        <div
          class="block flex-col mb-8 lg:mb-16 space-y-4 sm:flex-row sm:justify-center sm:space-y-0 sm:space-x-4"
        >
          <a
            href="#"
            class="inline-flex justify-center items-center py-3 px-5 text-base font-medium text-center text-gray-900 rounded-lg border border-gray-300 hover:bg-gray-100 focus:ring-4 focus:ring-gray-100 dark:text-white dark:border-gray-700 dark:hover:bg-gray-700 dark:focus:ring-gray-800"
          >
            <svg
              class="mr-2 -ml-1 w-5 h-5"
              fill="#7E22CE"
              viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M2 6a2 2 0 012-2h6a2 2 0 012 2v8a2 2 0 01-2 2H4a2 2 0 01-2-2V6zM14.553 7.106A1 1 0 0014 8v4a1 1 0 00.553.894l2 1A1 1 0 0018 13V7a1 1 0 00-1.447-.894l-2 1z"
              ></path>
            </svg>
            Watch video
          </a>
        </div>
      </div>

      <div class="lg:col-span-5">
        <img class="max-w-full h-auto" src="./public/imggroupclean.jpg" />
      </div>
    </div>
  </section>
  <!-- Hero2 -->

  <section class="bg-white dark:bg-gray-900">
    <div data-aos="fade-right">
      <div
        class="grid max-w-screen-4xl py-8 mx-auto xl:gap-0 lg:py-4 lg:grid-cols-12"
      >
        <div class="lg:col-span-5">
          <img class="hidden sm:block" src="./public/qrappmenu2.png" />
        </div>
        <div class="place-self-center grid lg:col-span-7">
          <h1
            class="max-w-5xl mb-4 text-4xl font-extrabold text-center tracking-tight leading-none md:text-5xl xl:text-6xl dark:text-white"
          >
            Un <span style="color: #7e22ce">écosystème digitale </span>dédie à
            la <br />restauration
          </h1>
          <p
            class="max-w-4xl mb-6 font-light text-gray-500 text-center lg:mb-8 md:text-lg lg:text-xl dark:text-gray-400"
          >
            La platforme ultime pour une expérience de restauration sans
            friction. <br />
            Un simple scan du QR Code pour acceder au menu et realiser la prise
            de commmande. <br />
            Un suivi de la préparation de la commande en temps réel. <br />
            Un service à table fluide et accelerer.
          </p>
          <!-- <div
            class="inline-flex mx-auto justify-center items-center py-1 px-1 pr-4 mb-7 text-sm text-gray-700 bg-gray-100 rounded-full dark:bg-gray-800 dark:text-white hover:bg-gray-200 dark:hover:bg-gray-700"
          >
            <div
              id="slide"
              class="inline-flex mx-auto justify-center items-center"
            >
              <div
                class="text-xs bg-primary-600 rounded-full text-white px-4 py-1.5 mr-3"
              >
                <img class="w-6 h-6" src="./public/arrowleft.svg" />
              </div>
              <span class="text-xl font-medium"
                >Commencez l'aventure maintenant !</span
              >
            </div>
          </div> -->
          <div
            class="inline-flex mx-auto justify-center items-center py-1 px-1 pr-4 mb-7 text-sm text-gray-700 bg-gray-100 rounded-full dark:bg-gray-800 dark:text-white hover:bg-gray-200 dark:hover:bg-gray-700"
          >
            <div class="slide-container" @click="toggleSlide">
              <div
                id="slide"
                style="margin-right: 1em"
                class="text-xs bg-primary-600 rounded-full text-white px-4 py-1.5"
                :class="{ 'slide-right': isSlideRight }"
              >
                <img class="w-6 h-6" src="./public/arrowleft.svg" />
              </div>
              <span
                class="text-xl font-medium"
                :class="{ 'hide-text': isSlideRight }"
                >Commencez l'aventure maintenant !</span
              >
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!--Hero3-->
  <section class="bg-white h-auto dark:bg-gray-900">
    <div class="grid lg:mt-0 lg:grid-cols-12">
      <div class="py-8 max-w-screen-xl text-center lg:col-span-5">
        <h1
          class="max-w-5xl mb-4 mx-auto text-4xl font-extrabold text-center tracking-tight leading-none md:text-5xl xl:text-6xl dark:text-white"
        >
          Une <span style="color: #7e22ce"> gestion</span> simplifié
          <!-- Révolutionnez l'expérience de commande de votre restaurant -->
        </h1>
        <p
          class="mb-8 text-lg font-normal text-center text-gray-500 lg:text-xl sm:px-8 xl:px-8 dark:text-gray-400"
        >
          Le système de gestion que nous avons choisi de développer constitue le
          pilier central de votre stratégie d'entreprise. En plaçant notre
          solution au cœur de votre activité, vous bénéficiez d'un outil
          puissant et adapté qui optimisera vos opérations et renforcera votre
          efficacité.
        </p>
        <div class="mx-auto mt-16 max-w-2xl sm:mt-20 lg:mt-24 lg:max-w-4xl">
          <div class="flex flex-col max-w-xl gap-x-8 gap-y-10 lg:max-w-none">
            <div
              v-for="feature in features"
              :key="feature.name"
              class="grid lg:grid-cols-12"
            >
              <div
                class="lg:col-span-5 flex justify-center items-center sm:col-span-5"
              >
                <img :src="feature.imgPath" alt="" class="max-w-full h-auto" />
              </div>
              <div class="lg:col-span-5 lg:w-[432px] sm:mx-auto">
                <div
                  class="text-xl sm:text-center lg:text-left font-semibold leading-7 text-gray-900"
                >
                  {{ feature.name }}
                </div>
                <div
                  class="mt-2 text-base sm:text-center lg:text-left leading-7 text-gray-600"
                >
                  {{ feature.description }}
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="lg:col-span-7 py-32">
        <img
          class="max-w-full h-auto w-1/1 mx-auto"
          src="./public/appscreen.svg"
        />
      </div>
    </div>
  </section>
  <!-- Features -->
  <section>
    <div data-aos="fade-down">
      <div>
        <div class="mx-auto max-w-7xl px-6 lg:px-8">
          <div class="mx-auto max-w-2xl lg:text-center">
            <h2 class="text-base font-semibold leading-7 text-indigo-600">
              Deploy faster
            </h2>
            <p
              class="mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl"
            >
              Everything you need to deploy your app
            </p>
            <p class="mt-6 text-lg leading-8 text-gray-600">
              Quis tellus eget adipiscing convallis sit sit eget aliquet quis.
              Suspendisse eget egestas a elementum pulvinar et feugiat blandit
              at. In mi viverra elit nunc.
            </p>
          </div>
          <div class="mx-auto mt-16 max-w-2xl sm:mt-20 lg:mt-24 lg:max-w-4xl">
            <dl
              class="grid max-w-xl grid-cols-1 gap-x-8 gap-y-10 lg:max-w-none lg:grid-cols-2 lg:gap-y-16"
            >
              <div
                v-for="feature in features"
                :key="feature.name"
                class="relative pl-16"
              >
                <dt class="text-base font-semibold leading-7 text-gray-900">
                  <div
                    class="absolute left-0 top-0 flex h-10 w-10 items-center justify-center rounded-lg bg-indigo-600"
                  >
                    <component
                      :is="feature.icon"
                      class="h-6 w-6 text-white"
                      aria-hidden="true"
                    />
                  </div>
                  {{ feature.name }}
                </dt>
                <dd class="mt-2 text-base leading-7 text-gray-600">
                  {{ feature.description }}
                </dd>
              </div>
            </dl>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- stats -->
  <section>
    <div data-aos="fade-left">
      <div class="bg-white py-24 sm:py-32">
        <div class="mx-auto max-w-7xl px-6 lg:px-8">
          <dl
            class="grid grid-cols-1 gap-x-8 gap-y-16 text-center lg:grid-cols-3"
          >
            <div
              v-for="stat in stats"
              :key="stat.id"
              class="mx-auto flex max-w-xs flex-col gap-y-4"
            >
              <dt class="text-base leading-7 text-gray-600">{{ stat.name }}</dt>
              <dd
                class="order-first text-3xl font-semibold tracking-tight text-gray-900 sm:text-5xl"
              >
                {{ stat.value }}
              </dd>
            </div>
          </dl>
        </div>
      </div>
    </div>
  </section>
  <!-- Testimonials -->
  <section
    class="relative isolate overflow-hidden bg-white px-6 py-24 sm:py-32 lg:px-8"
  >
    <div
      class="absolute inset-0 -z-10 bg-[radial-gradient(45rem_50rem_at_top,theme(colors.indigo.100),white)] opacity-20"
    />
    <div
      class="absolute inset-y-0 right-1/2 -z-10 mr-16 w-[200%] origin-bottom-left skew-x-[-30deg] bg-white shadow-xl shadow-indigo-600/10 ring-1 ring-indigo-50 sm:mr-28 lg:mr-0 xl:mr-16 xl:origin-center"
    />
    <div class="mx-auto max-w-2xl lg:max-w-4xl">
      <img
        class="mx-auto h-12"
        src="https://tailwindui.com/img/logos/workcation-logo-indigo-600.svg"
        alt=""
      />
      <figure class="mt-10">
        <blockquote
          class="text-center text-xl font-semibold leading-8 text-gray-900 sm:text-2xl sm:leading-9"
        >
          <p>
            “Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo
            expedita voluptas culpa sapiente alias molestiae. Numquam corrupti
            in laborum sed rerum et corporis.”
          </p>
        </blockquote>
        <figcaption class="mt-10">
          <img
            class="mx-auto h-10 w-10 rounded-full"
            src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
            alt=""
          />
          <div
            class="mt-4 flex items-center justify-center space-x-3 text-base"
          >
            <div class="font-semibold text-gray-900">Judith Black</div>
            <svg
              viewBox="0 0 2 2"
              width="3"
              height="3"
              aria-hidden="true"
              class="fill-gray-900"
            >
              <circle cx="1" cy="1" r="1" />
            </svg>
            <div class="text-gray-600">CEO of Workcation</div>
          </div>
        </figcaption>
      </figure>
    </div>
  </section>
  <!-- contact -->
  <section class="bg-white dark:bg-gray-900">
    <div class="py-8 lg:py-16 px-4 mx-auto max-w-screen-md">
      <h2
        class="mb-4 text-4xl tracking-tight font-extrabold text-center text-gray-900 dark:text-white"
      >
        Contact Us
      </h2>
      <p
        class="mb-8 lg:mb-16 font-light text-center text-gray-500 dark:text-gray-400 sm:text-xl"
      >
        Got a technical issue? Want to send feedback about a beta feature? Need
        details about our Business plan? Let us know.
      </p>
      <form action="#" class="space-y-8">
        <div>
          <label
            for="email"
            class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300"
            >Your email</label
          >
          <input
            type="email"
            id="email"
            class="shadow-sm bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-primary-500 focus:border-primary-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500 dark:shadow-sm-light"
            placeholder="name@flowbite.com"
            required
          />
        </div>
        <div>
          <label
            for="subject"
            class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300"
            >Subject</label
          >
          <input
            type="text"
            id="subject"
            class="block p-3 w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300 shadow-sm focus:ring-primary-500 focus:border-primary-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500 dark:shadow-sm-light"
            placeholder="Let us know how we can help you"
            required
          />
        </div>
        <div class="sm:col-span-2">
          <label
            for="message"
            class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-400"
            >Your message</label
          >
          <textarea
            id="message"
            rows="6"
            class="block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-lg shadow-sm border border-gray-300 focus:ring-primary-500 focus:border-primary-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500"
            placeholder="Leave a comment..."
          ></textarea>
        </div>
        <button
          type="submit"
          class="py-3 px-5 text-sm font-medium text-center text-white rounded-lg bg-primary-700 sm:w-fit hover:bg-primary-800 focus:ring-4 focus:outline-none focus:ring-primary-300 dark:bg-primary-600 dark:hover:bg-primary-700 dark:focus:ring-primary-800"
        >
          Send messages
        </button>
      </form>
    </div>
  </section>
  <!-- Footer -->

  <section>
    <footer class="p-4 bg-white sm:p-6 dark:bg-gray-800">
      <div class="mx-auto max-w-screen-xl">
        <div class="md:flex md:justify-between">
          <div class="mb-6 md:mb-0">
            <a href="https://flowbite.com" class="flex items-center">
              <img
                src="https://flowbite.com/docs/images/logo.svg"
                class="mr-3 h-8"
                alt="FlowBite Logo"
              />
              <span
                class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white"
                >Flowbite</span
              >
            </a>
          </div>
          <div class="grid grid-cols-2 gap-8 sm:gap-6 sm:grid-cols-3">
            <div>
              <h2
                class="mb-6 text-sm font-semibold text-gray-900 uppercase dark:text-white"
              >
                Resources
              </h2>
              <ul class="text-gray-600 dark:text-gray-400">
                <li class="mb-4">
                  <a href="https://flowbite.com" class="hover:underline"
                    >Flowbite</a
                  >
                </li>
                <li>
                  <a href="https://tailwindcss.com/" class="hover:underline"
                    >Tailwind CSS</a
                  >
                </li>
              </ul>
            </div>
            <div>
              <h2
                class="mb-6 text-sm font-semibold text-gray-900 uppercase dark:text-white"
              >
                Follow us
              </h2>
              <ul class="text-gray-600 dark:text-gray-400">
                <li class="mb-4">
                  <a
                    href="https://github.com/themesberg/flowbite"
                    class="hover:underline"
                    >Github</a
                  >
                </li>
                <li>
                  <a
                    href="https://discord.gg/4eeurUVvTy"
                    class="hover:underline"
                    >Discord</a
                  >
                </li>
              </ul>
            </div>
            <div>
              <h2
                class="mb-6 text-sm font-semibold text-gray-900 uppercase dark:text-white"
              >
                Legal
              </h2>
              <ul class="text-gray-600 dark:text-gray-400">
                <li class="mb-4">
                  <a href="#" class="hover:underline">Privacy Policy</a>
                </li>
                <li>
                  <a href="#" class="hover:underline">Terms &amp; Conditions</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <hr
          class="my-6 border-gray-200 sm:mx-auto dark:border-gray-700 lg:my-8"
        />
        <div class="sm:flex sm:items-center sm:justify-between">
          <span class="text-sm text-gray-500 sm:text-center dark:text-gray-400"
            >© 2022
            <a href="https://flowbite.com" class="hover:underline">Flowbite™</a
            >. All Rights Reserved.
          </span>
          <div class="flex mt-4 space-x-6 sm:justify-center sm:mt-0">
            <a
              href="#"
              class="text-gray-500 hover:text-gray-900 dark:hover:text-white"
            >
              <svg
                class="w-5 h-5"
                fill="currentColor"
                viewBox="0 0 24 24"
                aria-hidden="true"
              >
                <path
                  fill-rule="evenodd"
                  d="M22 12c0-5.523-4.477-10-10-10S2 6.477 2 12c0 4.991 3.657 9.128 8.438 9.878v-6.987h-2.54V12h2.54V9.797c0-2.506 1.492-3.89 3.777-3.89 1.094 0 2.238.195 2.238.195v2.46h-1.26c-1.243 0-1.63.771-1.63 1.562V12h2.773l-.443 2.89h-2.33v6.988C18.343 21.128 22 16.991 22 12z"
                  clip-rule="evenodd"
                />
              </svg>
            </a>
            <a
              href="#"
              class="text-gray-500 hover:text-gray-900 dark:hover:text-white"
            >
              <svg
                class="w-5 h-5"
                fill="currentColor"
                viewBox="0 0 24 24"
                aria-hidden="true"
              >
                <path
                  fill-rule="evenodd"
                  d="M12.315 2c2.43 0 2.784.013 3.808.06 1.064.049 1.791.218 2.427.465a4.902 4.902 0 011.772 1.153 4.902 4.902 0 011.153 1.772c.247.636.416 1.363.465 2.427.048 1.067.06 1.407.06 4.123v.08c0 2.643-.012 2.987-.06 4.043-.049 1.064-.218 1.791-.465 2.427a4.902 4.902 0 01-1.153 1.772 4.902 4.902 0 01-1.772 1.153c-.636.247-1.363.416-2.427.465-1.067.048-1.407.06-4.123.06h-.08c-2.643 0-2.987-.012-4.043-.06-1.064-.049-1.791-.218-2.427-.465a4.902 4.902 0 01-1.772-1.153 4.902 4.902 0 01-1.153-1.772c-.247-.636-.416-1.363-.465-2.427-.047-1.024-.06-1.379-.06-3.808v-.63c0-2.43.013-2.784.06-3.808.049-1.064.218-1.791.465-2.427a4.902 4.902 0 011.153-1.772A4.902 4.902 0 015.45 2.525c.636-.247 1.363-.416 2.427-.465C8.901 2.013 9.256 2 11.685 2h.63zm-.081 1.802h-.468c-2.456 0-2.784.011-3.807.058-.975.045-1.504.207-1.857.344-.467.182-.8.398-1.15.748-.35.35-.566.683-.748 1.15-.137.353-.3.882-.344 1.857-.047 1.023-.058 1.351-.058 3.807v.468c0 2.456.011 2.784.058 3.807.045.975.207 1.504.344 1.857.182.466.399.8.748 1.15.35.35.683.566 1.15.748.353.137.882.3 1.857.344 1.054.048 1.37.058 4.041.058h.08c2.597 0 2.917-.01 3.96-.058.976-.045 1.505-.207 1.858-.344.466-.182.8-.398 1.15-.748.35-.35.566-.683.748-1.15.137-.353.3-.882.344-1.857.048-1.055.058-1.37.058-4.041v-.08c0-2.597-.01-2.917-.058-3.96-.045-.976-.207-1.505-.344-1.858a3.097 3.097 0 00-.748-1.15 3.098 3.098 0 00-1.15-.748c-.353-.137-.882-.3-1.857-.344-1.023-.047-1.351-.058-3.807-.058zM12 6.865a5.135 5.135 0 110 10.27 5.135 5.135 0 010-10.27zm0 1.802a3.333 3.333 0 100 6.666 3.333 3.333 0 000-6.666zm5.338-3.205a1.2 1.2 0 110 2.4 1.2 1.2 0 010-2.4z"
                  clip-rule="evenodd"
                />
              </svg>
            </a>
            <a
              href="#"
              class="text-gray-500 hover:text-gray-900 dark:hover:text-white"
            >
              <svg
                class="w-5 h-5"
                fill="currentColor"
                viewBox="0 0 24 24"
                aria-hidden="true"
              >
                <path
                  d="M8.29 20.251c7.547 0 11.675-6.253 11.675-11.675 0-.178 0-.355-.012-.53A8.348 8.348 0 0022 5.92a8.19 8.19 0 01-2.357.646 4.118 4.118 0 001.804-2.27 8.224 8.224 0 01-2.605.996 4.107 4.107 0 00-6.993 3.743 11.65 11.65 0 01-8.457-4.287 4.106 4.106 0 001.27 5.477A4.072 4.072 0 012.8 9.713v.052a4.105 4.105 0 003.292 4.022 4.095 4.095 0 01-1.853.07 4.108 4.108 0 003.834 2.85A8.233 8.233 0 012 18.407a11.616 11.616 0 006.29 1.84"
                />
              </svg>
            </a>
            <a
              href="#"
              class="text-gray-500 hover:text-gray-900 dark:hover:text-white"
            >
              <svg
                class="w-5 h-5"
                fill="currentColor"
                viewBox="0 0 24 24"
                aria-hidden="true"
              >
                <path
                  fill-rule="evenodd"
                  d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0022 12.017C22 6.484 17.522 2 12 2z"
                  clip-rule="evenodd"
                />
              </svg>
            </a>
            <a
              href="#"
              class="text-gray-500 hover:text-gray-900 dark:hover:text-white"
            >
              <svg
                class="w-5 h-5"
                fill="currentColor"
                viewBox="0 0 24 24"
                aria-hidden="true"
              >
                <path
                  fill-rule="evenodd"
                  d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10c5.51 0 10-4.48 10-10S17.51 2 12 2zm6.605 4.61a8.502 8.502 0 011.93 5.314c-.281-.054-3.101-.629-5.943-.271-.065-.141-.12-.293-.184-.445a25.416 25.416 0 00-.564-1.236c3.145-1.28 4.577-3.124 4.761-3.362zM12 3.475c2.17 0 4.154.813 5.662 2.148-.152.216-1.443 1.941-4.48 3.08-1.399-2.57-2.95-4.675-3.189-5A8.687 8.687 0 0112 3.475zm-3.633.803a53.896 53.896 0 013.167 4.935c-3.992 1.063-7.517 1.04-7.896 1.04a8.581 8.581 0 014.729-5.975zM3.453 12.01v-.26c.37.01 4.512.065 8.775-1.215.25.477.477.965.694 1.453-.109.033-.228.065-.336.098-4.404 1.42-6.747 5.303-6.942 5.629a8.522 8.522 0 01-2.19-5.705zM12 20.547a8.482 8.482 0 01-5.239-1.8c.152-.315 1.888-3.656 6.703-5.337.022-.01.033-.01.054-.022a35.318 35.318 0 011.823 6.475 8.4 8.4 0 01-3.341.684zm4.761-1.465c-.086-.52-.542-3.015-1.659-6.084 2.679-.423 5.022.271 5.314.369a8.468 8.468 0 01-3.655 5.715z"
                  clip-rule="evenodd"
                />
              </svg>
            </a>
          </div>
        </div>
      </div>
    </footer>
  </section>
</template>
<script setup>
import { ref } from "vue";
import AOS from "aos";
import "aos/dist/aos.css"; // You can also use <link> for styles
// ..
AOS.init({
  offset: 120, // offset (in px) from the original trigger point
  delay: 5, // values from 0 to 3000, with step 50ms
  duration: 1500, // values from 0 to 3000, with step 50ms
  easing: "ease", // default easing for AOS animations
  once: false, // whether animation should happen only once - while scrolling down
  mirror: false, // whether elements should animate out while scrolling past them
});

const navigation = [
  { name: "Product", href: "#" },
  { name: "Features", href: "#" },
  { name: "Marketplace", href: "#" },
  { name: "Company", href: "#" },
];

import {
  Dialog,
  DialogPanel,
  Disclosure,
  DisclosureButton,
  DisclosurePanel,
  Popover,
  PopoverButton,
  PopoverGroup,
  PopoverPanel,
} from "@headlessui/vue";
import {
  ArrowPathIcon,
  Bars3Icon,
  ChartPieIcon,
  CursorArrowRaysIcon,
  FingerPrintIcon,
  SquaresPlusIcon,
  LockClosedIcon,
  CloudArrowUpIcon,
  XMarkIcon,
} from "@heroicons/vue/24/outline";
import {
  ChevronDownIcon,
  PhoneIcon,
  PlayCircleIcon,
} from "@heroicons/vue/20/solid";

const products = [
  {
    name: "Analytics",
    description: "Get a better understanding of your traffic",
    href: "#",
    icon: ChartPieIcon,
  },
  {
    name: "Engagement",
    description: "Speak directly to your customers",
    href: "#",
    icon: CursorArrowRaysIcon,
  },
  {
    name: "Security",
    description: "Your customers’ data will be safe and secure",
    href: "#",
    icon: FingerPrintIcon,
  },
  {
    name: "Integrations",
    description: "Connect with third-party tools",
    href: "#",
    icon: SquaresPlusIcon,
  },
  {
    name: "Automations",
    description: "Build strategic funnels that will convert",
    href: "#",
    icon: ArrowPathIcon,
  },
];
const callsToAction = [
  { name: "Watch demo", href: "#", icon: PlayCircleIcon },
  { name: "Contact sales", href: "#", icon: PhoneIcon },
];
const features = [
  {
    name: "Prise de commande",
    description:
      "Notre système de gestion des commandes en temps réel vous permettra de suivre facilement les demandes, d’optimiser l’efficacité opérationnelle et de grantir une livraison rapide.",
    imgPath: "/prisedecommande.svg",
  },
  {
    name: "Inventaire des stocks",
    description:
      "Notre application vous offre une solution complète pour la gestion de l'inventaire des stocks, vous permettant ainsi d'avoir une vision claire et précise des produits disponibles.",
    imgPath: "/inventaire.svg",
  },
  {
    name: "Menu personnalisable",
    description:
      "Une interface conviviale et intuitive pour personnaliser votre menu simplement.  Modifiez vos plats, intégrer de nouvelles options, spécifier les ingrédients souhaités ou encore concevoir des menus sur mesure.",
    imgPath: "/menupersonnalisable.svg",
  },
];
const stats = [
  { id: 1, name: "Transactions every 24 hours", value: "44 million" },
  { id: 2, name: "Assets under holding", value: "$119 trillion" },
  { id: 3, name: "New users annually", value: "46,000" },
];
const mobileMenuOpen = ref(false);

const isSlideRight = ref(false);

function toggleSlide() {
  isSlideRight.value = !isSlideRight.value;
  setTimeout(() => {
    isSlideRight.value = false;
  }, 3000);
}
</script>

<style>
.slide-container {
  position: relative;
  display: inline-flex;
  align-items: center;
}

#slide {
  transition: transform 0.5s;
}

.slide-right {
  transform: translateX(620%);
}
.hide-text {
  opacity: 0;
  transition: opacity 0.3s;
}
</style>
