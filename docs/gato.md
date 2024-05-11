# Esto es un gato
 Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
 tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
 cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
 proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## Esto es otro tema


 Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
 tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
 cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
 proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

![gato](https://ca-times.brightspotcdn.com/dims4/default/796e6c9/2147483647/strip/true/crop/1970x1108+39+0/resize/1200x675!/quality/75/?url=https%3A%2F%2Fcalifornia-times-brightspot.s3.amazonaws.com%2F12%2Fa5%2F79e097ccf62312d18a025f22ce48%2Fhoyla-recuento-11-cosas-aman-gatos-top-001)


## Ahora un bloque de codigo

```js
<template>
  <ul class="grid grid-cols-1 xl:grid-cols-3 gap-y-10 gap-x-6 items-start p-8">
    <li v-for="post in posts.data" class="relative flex flex-col sm:flex-row xl:flex-col items-start bg-white rounded-lg  shadow-lg">
      <div class="order-1 sm:ml-6 xl:ml-0">
       <NuxtLink :to="post.categoria">
        <span class="mb-1 pl-4 block text-sm leading-6 text-indigo-500">{{ post.categoria }}</span>
       </NuxtLink>

        <h2 class="mb-1 pl-4 text-slate-900 font-semibold">
          {{ post.tituloSeo }}
        </h2>
        <div class="pl-4 prose prose-slate prose-sm text-slate-600">
          <p> {{ post.descripcionSeo }}</p>
        </div>
        <NuxtLink
          class="group inline-flex items-center h-9 rounded-full text-sm font-semibold whitespace-nowrap px-3 focus:outline-none focus:ring-2 bg-slate-100 text-slate-700 hover:bg-slate-200 hover:text-slate-900 focus:ring-slate-500 mt-6"
          :to="`/${post.categoria}/${post.urlSeo}`">Leer mas
          <svg class="overflow-visible ml-3 text-slate-300 group-hover:text-slate-400" width="3" height="6"
            viewBox="0 0 3 6" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"
            stroke-linejoin="round">
            <path d="M0 0L3 3L0 6"></path>
          </svg></NuxtLink>

          {{ post.like }} <UIcon name="i-heroicons-hand-thumb-up-20-solid" />

      </div>
      <NuxtImg :src="post.fotoPortada" :alt="post.titulo"
        class="mb-6 shadow-md rounded-lg bg-slate-50 w-full sm:w-[17rem] sm:mb-0 xl:mb-6 xl:w-full" width="1216"
        height="640"/>
    </li>

  </ul>

</template>

```