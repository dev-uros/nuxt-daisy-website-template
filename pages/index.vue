<script lang="ts" setup>


</script>

<template>

  <div>

    <!--Hero element-->
    <div
        class="hero h-96"
        style="background-image: url(https://img.daisyui.com/images/stock/photo-1507358522600-9f71e620c44e.webp);">
      <div class="hero-overlay bg-opacity-60"></div>
      <div class="hero-content text-neutral-content text-center">
        <div class="max-w-md">
          <h1 class="mb-5 text-5xl font-bold"><span class="text-primary">Website</span> <span class="text-secondary">Template</span></h1>
          <p class="mb-5">
            Provident cupiditate voluptatem et in. Quaerat fugiat ut assumenda excepturi exercitationem
            quasi. In deleniti eaque aut repudiandae et a id nisi.
          </p>
          <div class="flex gap-4 justify-evenly rounded-md border-2 p-7">
            <button class="btn btn-secondary">Services</button>

            <button class="btn btn-primary">Products</button>
          </div>
        </div>
      </div>

    </div>
    <!--Hero element-->


    <!--Content element-->
    <div>
      <ul class="timeline timeline-snap-icon max-md:timeline-compact timeline-vertical">
        <li>
          <div class="timeline-middle">
            <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 20 20"
                fill="currentColor"
                class="h-5 w-5">
              <path
                  fill-rule="evenodd"
                  d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
                  clip-rule="evenodd"/>
            </svg>
          </div>
          <div class="timeline-start mb-10 md:text-end">
            <time class="font-mono italic">Product 1</time>
            <div class="card lg:card-side bg-base-100 shadow-xl">
              <figure>
                <img
                    src="https://img.daisyui.com/images/stock/photo-1494232410401-ad00d5433cfa.webp"
                    alt="Album" />
              </figure>
              <div class="card-body">
                <h2 class="card-title">New album is released!</h2>
                <p>Click the button to listen on Spotiwhy app.</p>
                <div class="card-actions justify-end">
                  <button class="btn btn-primary">Listen</button>
                </div>
              </div>
            </div>

          </div>
          <hr/>
        </li>
        <li>
          <hr/>
          <div class="timeline-middle">
            <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 20 20"
                fill="currentColor"
                class="h-5 w-5">
              <path
                  fill-rule="evenodd"
                  d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
                  clip-rule="evenodd"/>
            </svg>
          </div>
          <div class="timeline-end mb-10">
            <time class="font-mono italic">Product 2</time>
            <div class="card card-side bg-base-100 shadow-xl">
              <figure>
                <img
                    src="https://img.daisyui.com/images/stock/photo-1635805737707-575885ab0820.webp"
                    alt="Movie" />
              </figure>
              <div class="card-body">
                <h2 class="card-title">New movie is released!</h2>
                <p>Click the button to watch on Jetflix app.</p>
                <div class="card-actions justify-end">
                  <button class="btn btn-primary">Watch</button>
                </div>
              </div>
            </div>
          </div>
          <hr/>
        </li>
        <li>
          <hr/>
          <div class="timeline-middle">
            <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 20 20"
                fill="currentColor"
                class="h-5 w-5">
              <path
                  fill-rule="evenodd"
                  d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
                  clip-rule="evenodd"/>
            </svg>
          </div>
          <div class="timeline-start mb-10 md:text-end">
            <time class="font-mono italic">Product 3</time>
            <div class="card glass w-96">
              <figure>
                <img
                    src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
                    alt="car!" />
              </figure>
              <div class="card-body">
                <h2 class="card-title">Life hack</h2>
                <p>How to park your car at your garage?</p>
                <div class="card-actions justify-end">
                  <button class="btn btn-primary">Learn now!</button>
                </div>
              </div>
            </div>
          </div>
          <hr/>
        </li>
        <li>
          <hr/>
          <div class="timeline-middle">
            <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 20 20"
                fill="currentColor"
                class="h-5 w-5">
              <path
                  fill-rule="evenodd"
                  d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
                  clip-rule="evenodd"/>
            </svg>
          </div>
          <div class="timeline-end mb-10">
            <time class="font-mono italic">Service 1</time>
            <div class="card">
              <div class="card-title">
                Browse through Service 1 capabilities
              </div>
              <div class="card-body">
                <div class="carousel carousel-vertical rounded-box h-96">
                  <div class="carousel-item h-full">
                    <img src="https://img.daisyui.com/images/stock/photo-1559703248-dcaaec9fab78.webp" />
                  </div>
                  <div class="carousel-item h-full">
                    <img src="https://img.daisyui.com/images/stock/photo-1565098772267-60af42b81ef2.webp" />
                  </div>
                  <div class="carousel-item h-full">
                    <img src="https://img.daisyui.com/images/stock/photo-1572635148818-ef6fd45eb394.webp" />
                  </div>
                  <div class="carousel-item h-full">
                    <img src="https://img.daisyui.com/images/stock/photo-1494253109108-2e30c049369b.webp" />
                  </div>
                  <div class="carousel-item h-full">
                    <img src="https://img.daisyui.com/images/stock/photo-1550258987-190a2d41a8ba.webp" />
                  </div>
                  <div class="carousel-item h-full">
                    <img src="https://img.daisyui.com/images/stock/photo-1559181567-c3190ca9959b.webp" />
                  </div>
                  <div class="carousel-item h-full">
                    <img src="https://img.daisyui.com/images/stock/photo-1601004890684-d8cbf643f5f2.webp" />
                  </div>
                </div>
              </div>
            </div>

          </div>
          <hr/>
        </li>
        <li>
          <hr/>
          <div class="timeline-middle">
            <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 20 20"
                fill="currentColor"
                class="h-5 w-5">
              <path
                  fill-rule="evenodd"
                  d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
                  clip-rule="evenodd"/>
            </svg>
          </div>
          <div class="timeline-start mb-10 md:text-end">
            <time class="font-mono italic">Service 2</time>

            <div class="text-lg font-black">Service 2 title</div>
            Service 2 does stuff, and these are some stats on how the stuff is done!
            <div class="stats shadow">
              <div class="stat">
                <div class="stat-figure text-primary">
                  <svg
                      xmlns="http://www.w3.org/2000/svg"
                      fill="none"
                      viewBox="0 0 24 24"
                      class="inline-block h-8 w-8 stroke-current">
                    <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"></path>
                  </svg>
                </div>
                <div class="stat-title">Total Likes</div>
                <div class="stat-value text-primary">25.6K</div>
                <div class="stat-desc">21% more than last month</div>
              </div>

              <div class="stat">
                <div class="stat-figure text-secondary">
                  <svg
                      xmlns="http://www.w3.org/2000/svg"
                      fill="none"
                      viewBox="0 0 24 24"
                      class="inline-block h-8 w-8 stroke-current">
                    <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M13 10V3L4 14h7v7l9-11h-7z"></path>
                  </svg>
                </div>
                <div class="stat-title">Page Views</div>
                <div class="stat-value text-secondary">2.6M</div>
                <div class="stat-desc">21% more than last month</div>
              </div>

              <div class="stat">
                <div class="stat-figure text-secondary">
                  <div class="avatar online">
                    <div class="w-16 rounded-full">
                      <img src="https://img.daisyui.com/images/stock/photo-1534528741775-53994a69daeb.webp" />
                    </div>
                  </div>
                </div>
                <div class="stat-value">86%</div>
                <div class="stat-title">Tasks done</div>
                <div class="stat-desc text-secondary">31 tasks remaining</div>
              </div>
            </div>
          </div>
        </li>
      </ul>
    </div>
    <!--Content element-->

  </div>
</template>

<style scoped></style>
