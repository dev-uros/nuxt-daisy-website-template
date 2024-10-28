<script lang="ts" setup>
import ServiceIcon from "~/components/icons/ServiceIcon.vue";
import ServiceWrenchIcon from "~/components/icons/ServiceWrenchIcon.vue";
import ServiceAnalyticsIcon from "~/components/icons/ServiceAnalyticsIcon.vue";
import ServiceConsultingIcon from "~/components/icons/ServiceConsultingIcon.vue";
</script>

<template>
  <div class="container mx-auto px-4">
    <div class="card border-2 rounded-xl p-2">
      <div class="card-title mx-auto prose">
        <ServiceIcon/>
        <h1>Services</h1>
      </div>
      <div class="card-body grid lg:grid-cols-3 md:grid-cols-1 sm:grid-cols-1">
        <div class="card border-8 p-4">
          <div class="card-title">
            <ServiceWrenchIcon/>
            Repairs
          </div>
          <div class="divider divider-primary"></div>
          <div class="card-body">
            <ul class="list-disc">
              <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut tempus nunc. Integer tempor,
                velit non posuere convallis, felis turpis placerat mi, sed eleifend metus mi eget turpis. Ut aliquet.
              </li>
              <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut tempus nunc. Integer tempor,
                velit non posuere convallis, felis turpis placerat mi, sed eleifend metus mi eget turpis. Ut aliquet.
              </li>
              <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut tempus nunc. Integer tempor,
                velit non posuere convallis, felis turpis placerat mi, sed eleifend metus mi eget turpis. Ut aliquet.
              </li>

            </ul>
          </div>
          <div class="card-actions justify-evenly">
            <button class="btn btn-secondary">More Info</button>
            <button class="btn btn-primary">Make Inquiry</button>
          </div>
        </div>
        <div class="card border-8 p-4">
          <div class="card-title">
            <ServiceAnalyticsIcon/>
            Analytics
          </div>
          <div class="divider divider-primary"></div>
          <div class="card-body">
            <ul class="list-disc">
              <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut tempus nunc. Integer tempor,
                velit non posuere convallis, felis turpis placerat mi, sed eleifend metus mi eget turpis. Ut aliquet.
              </li>
              <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut tempus nunc. Integer tempor,
                velit non posuere convallis, felis turpis placerat mi, sed eleifend metus mi eget turpis. Ut aliquet.
              </li>
              <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut tempus nunc. Integer tempor,
                velit non posuere convallis, felis turpis placerat mi, sed eleifend metus mi eget turpis. Ut aliquet.
              </li>
              <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut tempus nunc. Integer tempor,
                velit non posuere convallis, felis turpis placerat mi, sed eleifend metus mi eget turpis. Ut aliquet.
              </li>
              <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut tempus nunc. Integer tempor,
                velit non posuere convallis, felis turpis placerat mi, sed eleifend metus mi eget turpis. Ut aliquet.
              </li>
            </ul>
          </div>
          <div class="card-actions justify-evenly">
            <button class="btn btn-secondary">More Info</button>
            <button class="btn btn-primary">Make Inquiry</button>
          </div>
        </div>
        <div class="card border-8 p-4">
          <div class="card-title">
            <ServiceConsultingIcon/>
            Consulting
          </div>
          <div class="divider divider-primary"></div>
          <div class="card-body">
            <ul class="list-disc">
              <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut tempus nunc. Integer tempor,
                velit non posuere convallis, felis turpis placerat mi, sed eleifend metus mi eget turpis. Ut aliquet.
              </li>
              <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut tempus nunc. Integer tempor,
                velit non posuere convallis, felis turpis placerat mi, sed eleifend metus mi eget turpis. Ut aliquet.
              </li>
              <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut tempus nunc. Integer tempor,
                velit non posuere convallis, felis turpis placerat mi, sed eleifend metus mi eget turpis. Ut aliquet.
              </li>
              <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut tempus nunc. Integer tempor,
                velit non posuere convallis, felis turpis placerat mi, sed eleifend metus mi eget turpis. Ut aliquet.
              </li>

            </ul>

          </div>
          <div class="card-actions justify-evenly">
            <button class="btn btn-secondary">More Info</button>
            <button class="btn btn-primary">Make Inquiry</button>
          </div>
        </div>

      </div>
    </div>
  </div>
</template>

<style scoped></style>
