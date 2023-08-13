<script setup>
import Blog from './components/Blog.vue';

const blogs = [
  {
    title: 'The Magnificent Bogra',
    image: 'https://i.ibb.co/Kr4b0zJ/152013403-10158311889099633-8423107287930246533-o.jpg',
    description: 'Located in Rajshahi Division, Bogra is one of the oldest and most fascinating towns in Bangladesh',
    distance: '196 km from Dhaka',
    reviews: '16 reviews',
    slogan: 'Places to visit: Mahasthangarh, Vasu Bihar  Momo Inn'
  },
  {
    title: 'The Natural Beauty of Noakhali',
    image: 'https://2.bp.blogspot.com/-mo77szjfCxU/Vz2ZinNMFTI/AAAAAAAAKeU/97cc-LdgndgyT4RFGuqeLXLmK_vzuSsKwCKgB/s1600/Nijhum%2BSea%2BBeach.jpg',
    description: 'Located in Comilla Division, Noakhali is one of the oldest and most attractive towns in Bangladesh',
    distance: '171 km from Dhaka',
    reviews: '60 reviews',
    slogan: 'Places to visit: Nizum dwip, Vasu Bihar  Momo Inn'
  },
  {
    title: 'The Magnificent Coxbazar',
    image: 'https://media-cdn.tripadvisor.com/media/photo-s/0b/62/f0/ef/royal-tulip-sea-pearl.jpg',
    description: 'Located in Cittagong Division, Cox bazar is one of the oldest and tourist towns in Bangladesh',
    distance: '190 km from Dhaka',
    reviews: '66 reviews',
    slogan: 'Places to visit: Nizum dwip, Vasu Bihar  Momo Inn'
  },
  {
    title: 'The Port City Chittagong',
    image: 'https://upload.wikimedia.org/wikipedia/commons/thumb/2/26/Aerial_View_of_Shah_Amanat_Bridge_3.jpg/405px-Aerial_View_of_Shah_Amanat_Bridge_3.jpg',
    description: 'Located in Cittagong Division, Chittagong is one of the oldest and economic towns in Bangladesh',
    distance: '171 km from Dhaka',
    reviews: '35 reviews',
    slogan: 'Places to visit: Nizum dwip, Vasu Bihar  Momo Inn'
  },
]

</script>

<template>
  <section class="mx-auto ">
    <h1 class="my-10 text-center">Components</h1>
    
    <div class="flex flex-col space-y-5">

      <Blog v-for="(blog, index) in blogs" :key="index" v-bind="blog"/>

      <!-- <div class="w-full">
        <article class=" flex flex-wrap md:flex-nowrap shadow-lg mx-auto max-w-3xl group cursor-pointer transform duration-500 hover:-translate-y-1">
          <img class="w-full md:w-52" src="https://i.ibb.co/Kr4b0zJ/152013403-10158311889099633-8423107287930246533-o.jpg" alt="">
          <div class="">
            <div class="p-5 pb-10">
              <h1 class="text-2xl font-semibold text-gray-800 mt-4">
                The Magnificent Bogra
              </h1>
              <p class="text-xl text-gray-400 mt-2 leading-relaxed">
                Located in Rajshahi Division, Bogra is one of the oldest and most fascinating towns in Bangladesh
              </p>
            </div>
            <div class="bg-blue-50 p-5">
              <div class="sm:flex sm:justify-between">
                <div>
                  <div class="text-lg text-gray-700">
                    <span class="text-gray-900 font-bold">196 km</span> from Dhaka
                  </div>
                  <div class="flex items-center">
                    <div class="flex">
                      <svg class="w-4 h-4 mx-px fill-current text-green-600" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 14 14">
                        <path d="M6.43 12l-2.36 1.64a1 1 0 0 1-1.53-1.11l.83-2.75a1 1 0 0 0-.35-1.09L.73 6.96a1 1 0 0 1 .59-1.8l2.87-.06a1 1 0 0 0 .92-.67l.95-2.71a1 1 0 0 1 1.88 0l.95 2.71c.13.4.5.66.92.67l2.87.06a1 1 0 0 1 .59 1.8l-2.3 1.73a1 1 0 0 0-.34 1.09l.83 2.75a1 1 0 0 1-1.53 1.1L7.57 12a1 1 0 0 0-1.14 0z"></path>
                      </svg>
                      <svg class="w-4 h-4 mx-px fill-current text-green-600" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 14 14">
                        <path d="M6.43 12l-2.36 1.64a1 1 0 0 1-1.53-1.11l.83-2.75a1 1 0 0 0-.35-1.09L.73 6.96a1 1 0 0 1 .59-1.8l2.87-.06a1 1 0 0 0 .92-.67l.95-2.71a1 1 0 0 1 1.88 0l.95 2.71c.13.4.5.66.92.67l2.87.06a1 1 0 0 1 .59 1.8l-2.3 1.73a1 1 0 0 0-.34 1.09l.83 2.75a1 1 0 0 1-1.53 1.1L7.57 12a1 1 0 0 0-1.14 0z"></path>
                      </svg>
                      <svg class="w-4 h-4 mx-px fill-current text-green-600" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 14 14">
                        <path d="M6.43 12l-2.36 1.64a1 1 0 0 1-1.53-1.11l.83-2.75a1 1 0 0 0-.35-1.09L.73 6.96a1 1 0 0 1 .59-1.8l2.87-.06a1 1 0 0 0 .92-.67l.95-2.71a1 1 0 0 1 1.88 0l.95 2.71c.13.4.5.66.92.67l2.87.06a1 1 0 0 1 .59 1.8l-2.3 1.73a1 1 0 0 0-.34 1.09l.83 2.75a1 1 0 0 1-1.53 1.1L7.57 12a1 1 0 0 0-1.14 0z"></path>
                      </svg>
                      <svg class="w-4 h-4 mx-px fill-current text-green-600" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 14 14">
                        <path d="M6.43 12l-2.36 1.64a1 1 0 0 1-1.53-1.11l.83-2.75a1 1 0 0 0-.35-1.09L.73 6.96a1 1 0 0 1 .59-1.8l2.87-.06a1 1 0 0 0 .92-.67l.95-2.71a1 1 0 0 1 1.88 0l.95 2.71c.13.4.5.66.92.67l2.87.06a1 1 0 0 1 .59 1.8l-2.3 1.73a1 1 0 0 0-.34 1.09l.83 2.75a1 1 0 0 1-1.53 1.1L7.57 12a1 1 0 0 0-1.14 0z"></path>
                      </svg>
                      <svg class="w-4 h-4 mx-px fill-current text-green-600" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 14 14">
                        <path d="M6.43 12l-2.36 1.64a1 1 0 0 1-1.53-1.11l.83-2.75a1 1 0 0 0-.35-1.09L.73 6.96a1 1 0 0 1 .59-1.8l2.87-.06a1 1 0 0 0 .92-.67l.95-2.71a1 1 0 0 1 1.88 0l.95 2.71c.13.4.5.66.92.67l2.87.06a1 1 0 0 1 .59 1.8l-2.3 1.73a1 1 0 0 0-.34 1.09l.83 2.75a1 1 0 0 1-1.53 1.1L7.57 12a1 1 0 0 0-1.14 0z"></path>
                      </svg>
                    </div>
                    <div class="text-gray-600 ml-2 text-sm md:text-base mt-1">
                      16 reviews
                    </div>
                  </div>
                </div>
                <button type="button" class="bg-purple-700 text-white py-2 my-2 hover:bg-purple-600">Book Ticket</button>
              </div>
              <div class="mt-3 text-gray-600 text-sm md:text-sm">
                *Places to visit: Mahasthangarh, Vasu Bihar &amp; Momo Inn
              </div>
            </div>
          </div>
        </article>
      </div>
      <div class="w-full">
        <article class=" flex flex-wrap md:flex-nowrap shadow-lg mx-auto max-w-3xl group cursor-pointer transform duration-500 hover:-translate-y-1">
          <img class="w-full md:w-52" src="https://i.ibb.co/Kr4b0zJ/152013403-10158311889099633-8423107287930246533-o.jpg" alt="">
          <div class="">
            <div class="p-5 pb-10">
              <h1 class="text-2xl font-semibold text-gray-800 mt-4">
                The Magnificent Bogra
              </h1>
              <p class="text-xl text-gray-400 mt-2 leading-relaxed">
                Located in Rajshahi Division, Bogra is one of the oldest and most fascinating towns in Bangladesh
              </p>
            </div>
            <div class="bg-blue-50 p-5">
              <div class="sm:flex sm:justify-between">
                <div>
                  <div class="text-lg text-gray-700">
                    <span class="text-gray-900 font-bold">196 km</span> from Dhaka
                  </div>
                  <div class="flex items-center">
                    <div class="flex">
                      <svg class="w-4 h-4 mx-px fill-current text-green-600" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 14 14">
                        <path d="M6.43 12l-2.36 1.64a1 1 0 0 1-1.53-1.11l.83-2.75a1 1 0 0 0-.35-1.09L.73 6.96a1 1 0 0 1 .59-1.8l2.87-.06a1 1 0 0 0 .92-.67l.95-2.71a1 1 0 0 1 1.88 0l.95 2.71c.13.4.5.66.92.67l2.87.06a1 1 0 0 1 .59 1.8l-2.3 1.73a1 1 0 0 0-.34 1.09l.83 2.75a1 1 0 0 1-1.53 1.1L7.57 12a1 1 0 0 0-1.14 0z"></path>
                      </svg>
                      <svg class="w-4 h-4 mx-px fill-current text-green-600" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 14 14">
                        <path d="M6.43 12l-2.36 1.64a1 1 0 0 1-1.53-1.11l.83-2.75a1 1 0 0 0-.35-1.09L.73 6.96a1 1 0 0 1 .59-1.8l2.87-.06a1 1 0 0 0 .92-.67l.95-2.71a1 1 0 0 1 1.88 0l.95 2.71c.13.4.5.66.92.67l2.87.06a1 1 0 0 1 .59 1.8l-2.3 1.73a1 1 0 0 0-.34 1.09l.83 2.75a1 1 0 0 1-1.53 1.1L7.57 12a1 1 0 0 0-1.14 0z"></path>
                      </svg>
                      <svg class="w-4 h-4 mx-px fill-current text-green-600" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 14 14">
                        <path d="M6.43 12l-2.36 1.64a1 1 0 0 1-1.53-1.11l.83-2.75a1 1 0 0 0-.35-1.09L.73 6.96a1 1 0 0 1 .59-1.8l2.87-.06a1 1 0 0 0 .92-.67l.95-2.71a1 1 0 0 1 1.88 0l.95 2.71c.13.4.5.66.92.67l2.87.06a1 1 0 0 1 .59 1.8l-2.3 1.73a1 1 0 0 0-.34 1.09l.83 2.75a1 1 0 0 1-1.53 1.1L7.57 12a1 1 0 0 0-1.14 0z"></path>
                      </svg>
                      <svg class="w-4 h-4 mx-px fill-current text-green-600" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 14 14">
                        <path d="M6.43 12l-2.36 1.64a1 1 0 0 1-1.53-1.11l.83-2.75a1 1 0 0 0-.35-1.09L.73 6.96a1 1 0 0 1 .59-1.8l2.87-.06a1 1 0 0 0 .92-.67l.95-2.71a1 1 0 0 1 1.88 0l.95 2.71c.13.4.5.66.92.67l2.87.06a1 1 0 0 1 .59 1.8l-2.3 1.73a1 1 0 0 0-.34 1.09l.83 2.75a1 1 0 0 1-1.53 1.1L7.57 12a1 1 0 0 0-1.14 0z"></path>
                      </svg>
                      <svg class="w-4 h-4 mx-px fill-current text-green-600" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 14 14">
                        <path d="M6.43 12l-2.36 1.64a1 1 0 0 1-1.53-1.11l.83-2.75a1 1 0 0 0-.35-1.09L.73 6.96a1 1 0 0 1 .59-1.8l2.87-.06a1 1 0 0 0 .92-.67l.95-2.71a1 1 0 0 1 1.88 0l.95 2.71c.13.4.5.66.92.67l2.87.06a1 1 0 0 1 .59 1.8l-2.3 1.73a1 1 0 0 0-.34 1.09l.83 2.75a1 1 0 0 1-1.53 1.1L7.57 12a1 1 0 0 0-1.14 0z"></path>
                      </svg>
                    </div>
                    <div class="text-gray-600 ml-2 text-sm md:text-base mt-1">
                      16 reviews
                    </div>
                  </div>
                </div>
                <a href="#" class="mt-3 sm:mt-0 py-2 px-5 md:py-3 md:px-6 bg-purple-700 hover:bg-purple-600 font-bold text-white md:text-lg rounded-lg shadow-md">
                  Book Ticket
                </a>
              </div>
              <div class="mt-3 text-gray-600 text-sm md:text-sm">
                *Places to visit: Mahasthangarh, Vasu Bihar &amp; Momo Inn
              </div>
            </div>
          </div>
        </article>
      </div> -->
    </div>

  </section>
</template>

<style scoped></style>