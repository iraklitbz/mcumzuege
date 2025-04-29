<script setup>
const services = ref(
    [
      {
        name: 'Dienstleistungen',
        icon: 'fluent:home-12-filled',
        color: 'text-yellow-600',
      },
      {
        name: 'Umzug privat & gewerblich\n',
        icon: 'material-symbols:warehouse-rounded',
        color: 'text-blue-600',
      },
      {
        name: 'Möbelmontage',
        icon: 'map:furniture-store',
        color: 'text-green-600',
      },
      {
        name: 'Entrümpelung (Haus & wohnung)',
        icon: 'hugeicons:clean',
        color: 'text-orange-600',
      },
    ]
)
</script>
<template>
  <div>
    <header>
      <div class="bg-transparent  md:px-5 py-4 relative z-[998]">
        <div class="flex justify-center items-center w-[calc(100%_-_2.5rem)] lg:w-[calc(100%_-_3rem)] mx-auto max-w-xl md:max-w-7xl">
          <nuxt-link
            to="#"
            class="font-display text-4xl py-3 font-bold tracking-tighter text-blue-900 flex items-center justify-center gap-3"
          >
            <Icon name="hugeicons:house-03" size="1.6em" class="text-purple-950"  />
            M.C Umzüge
          </nuxt-link>
        </div>
      </div>
    </header>
    <div class="relative py-20 sm:pt-26 sm:pb-24">
      <div class="absolute inset-0 overflow-hidden bg-indigo-50 -top-36 -bottom-14">
        <nuxt-img alt="" class="absolute top-0 left-0 translate-x-[-55%] translate-y-[-10%] -scale-x-100 sm:left-1/2 sm:translate-x-[-98%] sm:translate-y-[-6%] lg:translate-x-[-106%] xl:translate-x-[-122%]" src="background.6c3571e0.jpg" />
        <div class="absolute inset-x-0 top-0 h-40 bg-linear-to-b from-white"></div>
        <div class="absolute inset-x-0 bottom-0 h-40 bg-linear-to-t from-white"></div>
      </div>

      <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8 relative">
        <div class="mx-auto max-w-2xl lg:max-w-4xl lg:px-12">
          <h1 class="font-display text-5xl font-bold tracking-tighter text-blue-600 sm:text-7xl">
            RUND UMS HAUS
          </h1>
          <h2 class="font-display text-2xl font-bold tracking-tighter text-blue-600 sm:text-3xl">Rundum Service fur ein schoneres Zuhause</h2>

          <div class="text-md flex flex-col gap-5 mt-5 text-blue-900 tracking-tighter">
            <p>Grundreinigung Unterhaltsreinigung, Terrassen und steinreinigung,Fensterreinigung, Haushaltshilfe, Teppich- und Polsterreinigung, Bauendreinigung, PV Anlagen Reinigung, Fassaden Reinigung, Treppenhaus Reinigung</p>
            <p>Regelmäßige Gartenpflege, Rasermähen, Hecken schneiden, Unkraut entfernen, Pflanzungen und Umgestaltungen, Erstellung von Beeten und Rabatten, Rasenansaat und -pflege, Winterdienst und Laubbeseitigung, und vieles mehr</p>
            <p>Gartenpflege und Landschaftsbau, Kleinreparaturen und Wartungsarbeiten, Reinigung von Treppenhäusern und Gemeinschaftsflächen, Winterdienst und Schneeraumung, Herbstdienst, Und vieles mehr</p>
            <p>Verpackungsservice, Transport von Möbeln und Kartons, Auf- und Abbau von Möbeln, Entsorgung von nicht mehr benötigten Gegenständen, Haushaltsauflösungen, und vieles mehr</p>
          </div>
          <div class="mt-6 space-y-6 font-display text-2xl tracking-tight text-blue-900">
            <p><strong>Contact:</strong></p>
            <a class="text-blue-600  flex item-center gap-2" href="mailto:info@mcumzuege.de">
              <Icon name="tabler:mail" size="1.2em" class="text-purple-950"  />
              info@mcumzuege.de
            </a>
            <a class="text-blue-600 flex item-center gap-2" href="tel:+491636800204">
              <Icon name="tabler:phone" size="1.2em" class="text-purple-950"  />
              +49 163 6800204
            </a>
            <p class="text-blue-600 flex item-center gap-2" href="tel:+491636800204">
              <Icon name="tabler:map-pin" size="1.2em" class="text-purple-950"  />
              Südstraße 111, 33647, Bielefeld
            </p>
          </div>

          <ul class="mt-10 text-2xl tracking-tight text-blue-900 grid grid-cols-2 gap-3">
            <li v-for="(item, index) in services" :key="index" class="flex flex-col items-center justify-center gap-3 py-10 px-5 bg-white rounded-2xl">
              <Icon :name="item.icon" size="2em" :class="item.color"  />
              {{
                item.name
              }}
            </li>
          </ul>


        </div>
      </div>
    </div>
  </div>
</template>
