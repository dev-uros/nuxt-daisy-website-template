<script lang="ts" setup>
import BlogIcon from "~/components/icons/BlogIcon.vue";

const pages = [1,2];
const currentPage = ref(1);

const setNextPage = () => {
  if(currentPage.value === 1){
    window.scrollTo(0, 0);
    currentPage.value = 2;
    return
  }

  return;
}

const setPreviousPage = () => {
  if(currentPage.value === 2){
    window.scrollTo(0, 0);
    currentPage.value = 1
    return;
  }

  return;
}
</script>

<template>
  <div class="container mx-auto px-4 py-4">
    <div class="card border-2 rounded-xl p-2">
      <div class="card-title mx-auto prose">
        <BlogIcon/>
        <h1>Blog</h1>
      </div>
      <div class="card-body flex flex-col">
        <div v-show="currentPage === 1" class="card card-side bg-base-100 shadow-xl">
          <figure>
            <img
                src="https://img.daisyui.com/images/stock/photo-1635805737707-575885ab0820.webp"
                alt="Movie" class="max-h-96 h-full"/>
          </figure>
          <div class="card-body">
            <h1 class="card-title">Blog post #5</h1>
            <div class="divider"></div>
            <p class="prose prose-2xl">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin at placerat dolor. Morbi maximus dui ut
              urna mattis condimentum. Sed pharetra lobortis faucibus. Mauris egestas turpis eu malesuada placerat.
              Nullam in ultricies nulla...
            </p>
            <div class="rating mt-4">
              <input type="radio" name="rating-4" class="mask mask-star-2 bg-green-500" disabled/>
              <input type="radio" name="rating-4" class="mask mask-star-2 bg-green-500"  disabled/>
              <input type="radio" name="rating-4" class="mask mask-star-2 bg-green-500" disabled/>
              <input type="radio" name="rating-4" class="mask mask-star-2 bg-green-500" disabled/>
              <input type="radio" name="rating-4" class="mask mask-star-2 bg-green-500" checked="checked" disabled/>
            </div>
            <div class="card-actions justify-between">
              <p class="prose prose-slate">Published at: 28.10.2024</p>
              <button class="btn btn-primary">Read more</button>
            </div>
          </div>
        </div>
        <div v-show="currentPage === 1" class="card card-side bg-base-100 shadow-xl">
          <div class="card-body">
            <h1 class="card-title">Blog post #4</h1>
            <div class="divider"></div>
            <p class="prose prose-2xl">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin at placerat dolor. Morbi maximus dui ut
              urna mattis condimentum. Sed pharetra lobortis faucibus. Mauris egestas turpis eu malesuada placerat.
              Nullam in ultricies nulla...
            </p>
            <div class="rating mt-4">
              <input type="radio" name="rating-4" class="mask mask-star-2 bg-orange-500" disabled/>
              <input type="radio" name="rating-4" class="mask mask-star-2 bg-orange-500"  />
              <input type="radio" name="rating-4" class="mask mask-star-2 bg-orange-500" checked="checked" disabled/>
              <input type="radio" name="rating-4" class="mask mask-star-2 bg-orange-500" disabled/>
              <input type="radio" name="rating-4" class="mask mask-star-2 bg-orange-500" disabled/>
            </div>

            <div class="card-actions justify-between">
              <p class="prose prose-slate">Published at: 28.10.2024</p>
              <button class="btn btn-primary">Read more</button>
            </div>
          </div>
          <figure>
            <img
                src="https://i.pinimg.com/736x/af/4b/f2/af4bf25a3cb7b13c32340428c1bf8243.jpg"
                alt="Movie" class="max-h-96 h-full"/>
          </figure>

        </div>
        <div v-show="currentPage === 1" class="card card-side bg-base-100 shadow-xl">
          <figure>
            <img
                src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQnqZ5UR5Ro1RPLliHBllhjQPw7JFujks_TGg&s"
                alt="Movie" class="max-h-96 h-full"/>
          </figure>
          <div class="card-body">
            <h1 class="card-title">Blog post #3</h1>
            <div class="divider"></div>
            <p class="prose prose-2xl">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin at placerat dolor. Morbi maximus dui ut
              urna mattis condimentum. Sed pharetra lobortis faucibus. Mauris egestas turpis eu malesuada placerat.
              Nullam in ultricies nulla...
            </p>
            <div class="rating mt-4">
              <input type="radio" name="rating-3" class="mask  mask-star-2 bg-red-500" checked="checked" disabled/>
              <input type="radio" name="rating-3" class="mask  mask-star-2 bg-red-500" disabled/>
              <input type="radio" name="rating-3" class="mask  mask-star-2 bg-red-500" disabled/>
              <input type="radio" name="rating-3" class="mask  mask-star-2 bg-red-500" disabled/>
              <input type="radio" name="rating-3" class="mask  mask-star-2 bg-red-500" disabled/>
            </div>

            <div class="card-actions justify-between">
              <p class="prose prose-slate">Published at: 28.10.2024</p>
              <button class="btn btn-primary">Read more</button>
            </div>
          </div>
        </div>
        <div v-show="currentPage === 2" class="card card-side bg-base-100 shadow-xl">
          <figure>
            <img
                src="https://image-cdn-ak.spotifycdn.com/image/ab67706c0000da84273b481181a8e042321dbf7c"
                alt="Movie" class="max-h-96 h-full"/>
          </figure>
          <div class="card-body">
            <h1 class="card-title">Blog post #2</h1>
            <div class="divider"></div>
            <p class="prose prose-2xl">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin at placerat dolor. Morbi maximus dui ut
              urna mattis condimentum. Sed pharetra lobortis faucibus. Mauris egestas turpis eu malesuada placerat.
              Nullam in ultricies nulla...
            </p>
            <div class="rating mt-4">
              <input type="radio" name="rating-2" class="mask  mask-star-2 bg-blue-500" disabled/>
              <input type="radio" name="rating-2" class="mask  mask-star-2 bg-blue-500" disabled/>
              <input type="radio" name="rating-2" class="mask  mask-star-2 bg-blue-500" disabled/>
              <input type="radio" name="rating-2" class="mask  mask-star-2 bg-blue-500" checked="checked" disabled/>
              <input type="radio" name="rating-2" class="mask  mask-star-2 bg-blue-500" disabled />
            </div>

            <div class="card-actions justify-between">
              <p class="prose prose-slate">Published at: 28.10.2024</p>
              <button class="btn btn-primary">Read more</button>
            </div>
          </div>
        </div>
        <div v-show="currentPage === 2" class="card card-side bg-base-100 shadow-xl">
          <figure>
            <img
                src="https://www.photomural.com/media/catalog/product/cache/2/thumbnail/9df78eab33525d08d6e5fb8d27136e95/I/A/IADX5-060.jpg"
                alt="Movie" class="max-h-96 h-full"/>
          </figure>
          <div class="card-body">
            <h1 class="card-title">Blog post #1</h1>
            <div class="divider"></div>
            <p class="prose prose-2xl">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin at placerat dolor. Morbi maximus dui ut
              urna mattis condimentum. Sed pharetra lobortis faucibus. Mauris egestas turpis eu malesuada placerat.
              Nullam in ultricies nulla...
            </p>
            <div class="rating mt-4">
              <input type="radio" name="rating-1" class="mask  mask-star-2 bg-yellow-500" disabled/>
              <input type="radio" name="rating-1" class="mask  mask-star-2 bg-yellow-500" checked="checked" disabled/>
              <input type="radio" name="rating-1" class="mask  mask-star-2 bg-yellow-500" disabled/>
              <input type="radio" name="rating-1" class="mask  mask-star-2 bg-yellow-500" disabled/>
              <input type="radio" name="rating-1" class="mask  mask-star-2 bg-yellow-500" disabled/>
            </div>

            <div class="card-actions justify-between">
              <p class="prose prose-slate">Published at: 28.10.2024</p>
              <button class="btn btn-primary">Read more</button>
            </div>
          </div>
        </div>

        <div class="join grid grid-cols-2 mt-4">
          <button class="join-item btn btn-outline" @click="setPreviousPage">Previous page</button>
          <button class="join-item btn btn-outline" @click="setNextPage">Next</button>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
