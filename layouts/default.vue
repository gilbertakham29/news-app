<template>
     <header>
    <nav class=" bg-indigo-200 border-gray-200 px-4 lg:px-6 py-2.5 dark:bg-gray-800">
        <div class="flex flex-wrap justify-between items-center mx-auto max-w-screen-xl">
            <NuxtLink to="/" class="flex items-center">
              
                <span class="self-center text-2xl text-green-500 font-semibold whitespace-nowrap dark:text-white">News-365</span>
            </NuxtLink>
            <button data-collapse-toggle="mobile-menu-2"  type="button" class="inline-flex lg:hidden items-center  p-2 ml-1 text-sm text-gray-500 rounded-lg  hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="mobile-menu-2" aria-expanded="false">
                    <span class="sr-only">Open main menu</span>
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd"></path></svg>
                    <svg class="hidden w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
                </button>
            <div class="hidden justify-between items-center w-full lg:flex lg:w-auto lg:order-1 " id="mobile-menu-2">
                <ul class="flex flex-col mt-4  font-medium lg:flex-row lg:space-x-8 lg:mt-0">
                    <li>
                        <a href="#" class=" py-2 pr-4 pl-3 text-white bg-black focus:ring-4 focus:ring-black font-light rounded-lg text-sm px-4 lg:px-5 lg:py-2.5 mr-2 dark:bg-primary-600 dark:hover:bg-primary-700 focus:outline-none dark:focus:ring-primary-800">All news</a>
                    </li>
                    <li>
                        <a href="#" class="block mt-1 py-2 pr-4 pl-3 text-gray-700 border-b border-gray-100 hover:bg-gray-50 font-light lg:hover:bg-transparent lg:border-0 lg:hover:text-primary-700 lg:p-0 dark:text-gray-400 lg:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white lg:dark:hover:bg-transparent dark:border-gray-700">Pricing</a>
                    </li>
                   
                    <li aria-labelledby="dropdownNavbarLink">
                    <button id="doubleDropdownButton" data-dropdown-toggle="doubleDropdown" data-dropdown-placement="right-start" type="button" class=" flex items-center justify-between mt-1 py-2 pr-4 pl-3 text-gray-700 border-b border-gray-100 hover:bg-gray-50 font-light lg:hover:bg-transparent lg:border-0 lg:hover:text-primary-700 lg:p-0 dark:text-gray-400 lg:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white lg:dark:hover:bg-transparent dark:border-gray-700">Categories<svg class="w-2.5 h-2.5 ml-2.5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 10 6">
    <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m1 1 4 4 4-4"/>
  </svg></button>
                    <div id="doubleDropdown" class="z-10 hidden bg-white divide-y divide-gray-100 rounded-lg shadow w-44 dark:bg-gray-700">
                        <ul class="py-2 text-sm text-gray-700 dark:text-gray-200" aria-labelledby="doubleDropdownButton">
                          <li>
                            <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-400 dark:hover:text-white">Action</a>
                          </li>
                          <li>
                            <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-400 dark:hover:text-white">Another Action</a>
                          </li>
                          <li>
                            <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-400 dark:hover:text-white">Something</a>
                          </li>
                          <li>
                            <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-400 dark:hover:text-white">Separated Link</a>
                          </li>
                        </ul>
                    </div>
                  </li>
                  <li class="lg:hidden">
                    
                        <img src="https://flowbite.com/docs/images/logo.svg" class="ml-1 mt-1 h-6 sm:h-9" alt="Flowbite Logo" />
                <a href="#" class="text-gray-800 dark:text-white  font-light rounded-lg text-sm px-2 lg:px-5 py-2 lg:py-2.5 mr-2 dark:hover:bg-gray-700 ">gilbert akham</a>
                <div class="flex flex-col">
                <a href="#" class="text-white text-center bg-red-700 hover:bg-red-800 focus:ring-4 focus:ring-red-300 font-medium rounded-lg text-sm px-4 lg:px-5 py-2 lg:py-2.5 mr-2 dark:bg-primary-600 dark:hover:bg-primary-700 focus:outline-none dark:focus:ring-primary-800">Log Out</a>
                <button data-collapse-toggle="mobile-menu-2"  type="button" class=" items-center lg:visible hidden p-2 ml-1 text-sm text-gray-500 rounded-lg  hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="mobile-menu-2" aria-expanded="false">
                    <span class="sr-only">Open main menu</span>
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd"></path></svg>
                    <svg class="hidden w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
                </button>
            </div>
                    </li>
                    <li class="lg:hidden">
                        <h1 class="text-2xl font-semibold text-black">All Category: 8</h1>
                        <div class="flex flex-col">
                <p class=" mt-3">
                    <NuxtLink to="/category/01" class=" text-blue-500 underline">Breaking News</NuxtLink>
                </p>
                <p class="mt-3">
                    <NuxtLink to="/category/02" class=" text-blue-500 underline">Regular News</NuxtLink>
                </p>
                <p class="mt-3">
                    <NuxtLink to="/category/03" class=" text-blue-500 underline">International News</NuxtLink>
                </p>
                <p class="mt-3">
                    <NuxtLink to="/category/04" class=" text-blue-500 underline">Sports</NuxtLink>
                </p>
                <p class="mt-3">
                    <NuxtLink to="/category/05" class=" text-blue-500 underline">Entertainment</NuxtLink>
                </p>
                <p class="mt-3">
                    <NuxtLink to="/category/06" class=" text-blue-500 underline">Culture</NuxtLink>
                </p>
                <p class="mt-3">
                    <NuxtLink to="/category/07" class=" text-blue-500 underline">Arts</NuxtLink>
                </p>
                <p class="mt-3">
                    <NuxtLink to="/category/08" class=" text-blue-500 underline">All News</NuxtLink>
                </p>
            </div>

                    </li>
                </ul>
            </div>
            <div class=" flex-col  lg:flex-row items-center lg:order-2 lg:flex hidden md:hidden sm:hidden">
                <img src="https://flowbite.com/docs/images/logo.svg" class="lg:visible h-6 sm:h-9" alt="Flowbite Logo" />
                <a href="#" class="text-gray-800 dark:text-white  font-light rounded-lg text-sm px-4 lg:px-5 py-2 lg:py-2.5 mr-2 dark:hover:bg-gray-700 ">gilbert akham</a>
                <a href="#" class="text-white bg-red-700 hover:bg-red-800 focus:ring-4 focus:ring-red-300 font-medium rounded-lg text-sm px-4 lg:px-5 py-2 lg:py-2.5 mr-2 dark:bg-primary-600 dark:hover:bg-primary-700 focus:outline-none dark:focus:ring-primary-800">Log Out</a>
                <button data-collapse-toggle="mobile-menu-2"  type="button" class=" items-center lg:visible hidden p-2 ml-1 text-sm text-gray-500 rounded-lg  hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="mobile-menu-2" aria-expanded="false">
                    <span class="sr-only">Open main menu</span>
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd"></path></svg>
                    <svg class="hidden w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
                </button>
            </div>
            
        </div>
    </nav>
</header>
    <div class="mt-12">

   
    <div class="lg:grid lg:grid-cols-3 flex flex-col">
        <div class="lg:flex flex-col justify-start items-start ml-24 hidden">
            <h1 class="text-2xl font-semibold text-black">All Category: 8</h1>
            <div class="flex flex-col">
                <p class=" mt-3">
                    <NuxtLink to="/category/01" class=" text-blue-500 underline">Breaking News</NuxtLink>
                </p>
                <p class="mt-3">
                    <NuxtLink to="/category/02" class=" text-blue-500 underline">Regular News</NuxtLink>
                </p>
                <p class="mt-3">
                    <NuxtLink to="/category/03" class=" text-blue-500 underline">International News</NuxtLink>
                </p>
                <p class="mt-3">
                    <NuxtLink to="/category/04" class=" text-blue-500 underline">Sports</NuxtLink>
                </p>
                <p class="mt-3">
                    <NuxtLink to="/category/05" class=" text-blue-500 underline">Entertainment</NuxtLink>
                </p>
                <p class="mt-3">
                    <NuxtLink to="/category/06" class=" text-blue-500 underline">Culture</NuxtLink>
                </p>
                <p class="mt-3">
                    <NuxtLink to="/category/07" class=" text-blue-500 underline">Arts</NuxtLink>
                </p>
                <p class="mt-3">
                    <NuxtLink to="/category/08" class=" text-blue-500 underline">All News</NuxtLink>
                </p>
            </div>
        </div>
       
        <slot/>
       <SocialSection/>
<Footer/>
       
    </div>
   
</div>

</template>