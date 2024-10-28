<script lang="ts" setup>
const setTheme = (theme: string) => {
  document.documentElement.setAttribute('data-theme', theme)
}
</script>

<template>
  <div class="flex flex-col min-h-screen">
    <div class="navbar bg-base-100">
      <div class="navbar-start">
        <div class="dropdown">
          <div tabindex="0" role="button" class="btn btn-ghost lg:hidden">
            <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-5 w-5"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor">
              <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M4 6h16M4 12h8m-8 6h16"/>
            </svg>
          </div>
          <ul
              tabindex="0"
              class="menu menu-sm dropdown-content bg-base-100 rounded-box z-[1] mt-3 w-52 p-2 shadow">
            <li><a>Item 1</a></li>
            <li>
              <a>Parent</a>
              <ul class="p-2">
                <li><a>Submenu 1</a></li>
                <li><a>Submenu 2</a></li>
              </ul>
            </li>
            <li><a>Item 3</a></li>
          </ul>
        </div>
        <div class="avatar">
          <div class="mask mask-hexagon w-12">
            <img
                src="https://media.istockphoto.com/id/851887036/vector/colorful-icon.jpg?s=612x612&w=0&k=20&c=a8kAIu0ZX6QnS99I8nQFMkTFlVYqFCnsugm54q-WX_s="/>
          </div>
        </div>
        <NuxtLink to="/" class="btn btn-ghost text-xl">Website Template</NuxtLink>
      </div>
      <div class="navbar-center hidden lg:flex">
        <ul class="menu menu-horizontal px-1">
          <li><NuxtLink to="/about" active-class="text-primary">About Us</NuxtLink></li>
          <li><NuxtLink to="/services" active-class="text-primary">Services</NuxtLink></li>
          <li><NuxtLink to="/products" active-class="text-primary">Products</NuxtLink></li>
          <li><NuxtLink to="/blog" active-class="text-primary">Blog</NuxtLink></li>
          <li><NuxtLink to="/faq" active-class="text-primary">FAQ</NuxtLink></li>
          <li><NuxtLink to="/contact" active-class="text-primary">Contact</NuxtLink></li>

        </ul>
      </div>
      <div class="navbar-end">
        <div class="dropdown dropdown-bottom dropdown-end ">
          <div tabindex="0" role="button" class="btn m-1">Theme Select</div>
          <ul tabindex="0"
              class="dropdown-content menu bg-base-100 rounded-box z-[1] p-4 shadow max-h-96 overflow-y-auto flex flex-row w-72 gap-2">
            <li data-theme="light" class="text-primary w-full" @click="setTheme('light')">
              <div>
                <span class="text-base">Light</span>
                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="dark" class="text-primary w-full" @click="setTheme('dark')">
              <div>
                <span class="text-base">Dark</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="cupcake" class="text-primary w-full" @click="setTheme('cupcake')">
              <div>
                <span class="text-base">Cupcake</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="bumblebee" class="text-primary w-full" @click="setTheme('bumblebee')">
              <div>
                <span class="text-base">Bumblebee</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="emerald" class="text-primary w-full" @click="setTheme('emerald')">
              <div>
                <span class="text-base">Emerald</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="corporate" class="text-primary w-full" @click="setTheme('corporate')">
              <div>
                <span class="text-base">Corporate</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="synthwave" class="text-primary w-full" @click="setTheme('synthwave')">
              <div>
                <span class="text-base">Synthwave</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="retro" class="text-primary w-full" @click="setTheme('retro')">
              <div>
                <span class="text-base">Retro</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="cyberpunk" class="text-primary w-full"  @click="setTheme('cyberpunk')">
              <div>
                <span class="text-base">Cyberpunk</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="valentine" class="text-primary w-full" @click="setTheme('valentine')">
              <div>
                <span class="text-base">Valentine</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="halloween" class="text-primary w-full" @click="setTheme('halloween')">
              <div>
                <span class="text-base">Halloween</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="garden" class="text-primary w-full" @click="setTheme('garden')">
              <div>
                <span class="text-base">Garden</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="forest" class="text-primary w-full" @click="setTheme('forest')">
              <div>
                <span class="text-base">Forest</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="aqua" class="text-primary w-full" @click="setTheme('aqua')">
              <div>
                <span class="text-base">Aqua</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="lofi" class="text-primary w-full" @click="setTheme('lofi')">
              <div>
                <span class="text-base">LoFi</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="pastel" class="text-primary w-full" @click="setTheme('pastel')">
              <div>
                <span class="text-base">Pastel</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="fantasy" class="text-primary w-full" @click="setTheme('fantasy')">
              <div>
                <span class="text-base">Fantasy</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="wireframe" class="text-primary w-full" @click="setTheme('wireframe')">
              <div>
                <span class="text-base">Wireframe</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="black" class="text-primary w-full" @click="setTheme('black')">
              <div>
                <span class="text-base">Black</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="luxury" class="text-primary w-full" @click="setTheme('luxury')">
              <div>
                <span class="text-base">Luxury</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="dracula" class="text-primary w-full" @click="setTheme('dracula')">
              <div>
                <span class="text-base">Dracula</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="cmyk" class="text-primary w-full" @click="setTheme('cmyk')">
              <div>
                <span class="text-base">Cmyk</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="autumn" class="text-primary w-full" @click="setTheme('autumn')">
              <div>
                <span class="text-base">Autumn</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="business" class="text-primary w-full" @click="setTheme('business')">
              <div>
                <span class="text-base">Business</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="acid" class="text-primary w-full" @click="setTheme('acid')">
              <div>
                <span class="text-base">Acid</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="lemonade" class="text-primary w-full" @click="setTheme('lemonade')">
              <div>
                <span class="text-base">Lemonade</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="night" class="text-primary w-full" @click="setTheme('night')">
              <div>
                <span class="text-base">Night</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="coffee" class="text-primary w-full" @click="setTheme('coffee')">
              <div>
                <span class="text-base">Coffee</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="winter" class="text-primary w-full" @click="setTheme('winter')">
              <div>
                <span class="text-base">Winter</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="dim" class="text-primary w-full" @click="setTheme('dim')">
              <div>
                <span class="text-base">Dim</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="nord" class="text-primary w-full" @click="setTheme('nord')">
              <div>
                <span class="text-base">Nord</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>
            <li data-theme="sunset" class="text-primary w-full" @click="setTheme('sunset')">
              <div>
                <span class="text-base">Sunset</span>

                <div class="flex gap-2 justify-end">
                  <div class="w-2 bg-primary">&nbsp</div>
                  <div class="w-2 bg-secondary">&nbsp</div>
                  <div class="w-2 bg-accent">&nbsp</div>
                  <div class="w-2 bg-neutral">&nbsp</div>
                  <div class="w-2 bg-info">&nbsp</div>
                  <div class="w-2 bg-success">&nbsp</div>
                  <div class="w-2 bg-warning">&nbsp</div>
                  <div class="w-2 bg-error">&nbsp</div>
                </div>
              </div>
            </li>

          </ul>
        </div>
        <!--        <a class="btn">Button</a>-->
      </div>
    </div>
    <!--    <header class="shadow-xl">-->
    <!--      <nav>-->
    <!--        <div class="navbar bg-base-100">-->
    <!--          <div class="navbar-start">-->
    <!--            <div class="dropdown">-->
    <!--              <div tabindex="0" role="button" class="btn btn-ghost btn-circle">-->
    <!--                <svg-->
    <!--                    xmlns="http://www.w3.org/2000/svg"-->
    <!--                    class="h-5 w-5"-->
    <!--                    fill="none"-->
    <!--                    viewBox="0 0 24 24"-->
    <!--                    stroke="currentColor">-->
    <!--                  <path-->
    <!--                      stroke-linecap="round"-->
    <!--                      stroke-linejoin="round"-->
    <!--                      stroke-width="2"-->
    <!--                      d="M4 6h16M4 12h16M4 18h7"/>-->
    <!--                </svg>-->
    <!--              </div>-->
    <!--              <ul-->
    <!--                  tabindex="0"-->
    <!--                  class="menu menu-sm dropdown-content bg-base-100 rounded-box z-[1] mt-3 w-52 p-2 shadow">-->
    <!--                <li><a>Homepage</a></li>-->
    <!--                <li><a>Portfolio</a></li>-->
    <!--                <li><a>About</a></li>-->
    <!--              </ul>-->
    <!--            </div>-->
    <!--          </div>-->
    <!--          <div class="navbar-center">-->
    <!--            <a class="btn btn-ghost text-xl">Website template</a>-->
    <!--          </div>-->
    <!--          <div class="navbar-end">-->
    <!--            <button class="btn btn-ghost btn-circle">-->
    <!--              <svg-->
    <!--                  xmlns="http://www.w3.org/2000/svg"-->
    <!--                  class="h-5 w-5"-->
    <!--                  fill="none"-->
    <!--                  viewBox="0 0 24 24"-->
    <!--                  stroke="currentColor">-->
    <!--                <path-->
    <!--                    stroke-linecap="round"-->
    <!--                    stroke-linejoin="round"-->
    <!--                    stroke-width="2"-->
    <!--                    d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"/>-->
    <!--              </svg>-->
    <!--            </button>-->
    <!--            <button class="btn btn-ghost btn-circle">-->
    <!--              <div class="indicator">-->
    <!--                <svg-->
    <!--                    xmlns="http://www.w3.org/2000/svg"-->
    <!--                    class="h-5 w-5"-->
    <!--                    fill="none"-->
    <!--                    viewBox="0 0 24 24"-->
    <!--                    stroke="currentColor">-->
    <!--                  <path-->
    <!--                      stroke-linecap="round"-->
    <!--                      stroke-linejoin="round"-->
    <!--                      stroke-width="2"-->
    <!--                      d="M15 17h5l-1.405-1.405A2.032 2.032 0 0118 14.158V11a6.002 6.002 0 00-4-5.659V5a2 2 0 10-4 0v.341C7.67 6.165 6 8.388 6 11v3.159c0 .538-.214 1.055-.595 1.436L4 17h5m6 0v1a3 3 0 11-6 0v-1m6 0H9"/>-->
    <!--                </svg>-->
    <!--                <span class="badge badge-xs badge-primary indicator-item"></span>-->
    <!--              </div>-->
    <!--            </button>-->
    <!--          </div>-->
    <!--        </div>-->
    <!--      </nav>-->
    <!--    </header>-->
    <main class="flex flex-grow">
      <slot/>

    </main>
    <footer class="footer bg-neutral text-neutral-content items-center p-4">
      <aside class="grid-flow-col items-center">
        <svg
            width="36"
            height="36"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
            fill-rule="evenodd"
            clip-rule="evenodd"
            class="fill-current">
          <path
              d="M22.672 15.226l-2.432.811.841 2.515c.33 1.019-.209 2.127-1.23 2.456-1.15.325-2.148-.321-2.463-1.226l-.84-2.518-5.013 1.677.84 2.517c.391 1.203-.434 2.542-1.831 2.542-.88 0-1.601-.564-1.86-1.314l-.842-2.516-2.431.809c-1.135.328-2.145-.317-2.463-1.229-.329-1.018.211-2.127 1.231-2.456l2.432-.809-1.621-4.823-2.432.808c-1.355.384-2.558-.59-2.558-1.839 0-.817.509-1.582 1.327-1.846l2.433-.809-.842-2.515c-.33-1.02.211-2.129 1.232-2.458 1.02-.329 2.13.209 2.461 1.229l.842 2.515 5.011-1.677-.839-2.517c-.403-1.238.484-2.553 1.843-2.553.819 0 1.585.509 1.85 1.326l.841 2.517 2.431-.81c1.02-.33 2.131.211 2.461 1.229.332 1.018-.21 2.126-1.23 2.456l-2.433.809 1.622 4.823 2.433-.809c1.242-.401 2.557.484 2.557 1.838 0 .819-.51 1.583-1.328 1.847m-8.992-6.428l-5.01 1.675 1.619 4.828 5.011-1.674-1.62-4.829z"></path>
        </svg>
        <p>Copyright © NuxtLink - All right reserved</p>
      </aside>
      <nav class="grid-flow-col gap-4 md:place-self-center md:justify-self-end">
        <a>
          <svg
              xmlns="http://www.w3.org/2000/svg"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              class="fill-current">
            <path
                d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z"></path>
          </svg>
        </a>
        <a>
          <svg
              xmlns="http://www.w3.org/2000/svg"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              class="fill-current">
            <path
                d="M19.615 3.184c-3.604-.246-11.631-.245-15.23 0-3.897.266-4.356 2.62-4.385 8.816.029 6.185.484 8.549 4.385 8.816 3.6.245 11.626.246 15.23 0 3.897-.266 4.356-2.62 4.385-8.816-.029-6.185-.484-8.549-4.385-8.816zm-10.615 12.816v-8l8 3.993-8 4.007z"></path>
          </svg>
        </a>
        <a>
          <svg
              xmlns="http://www.w3.org/2000/svg"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              class="fill-current">
            <path
                d="M9 8h-3v4h3v12h5v-12h3.642l.358-4h-4v-1.667c0-.955.192-1.333 1.115-1.333h2.885v-5h-3.808c-3.596 0-5.192 1.583-5.192 4.615v3.385z"></path>
          </svg>
        </a>
      </nav>
    </footer>
  </div>
</template>


<style scoped></style>
