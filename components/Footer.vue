<template>
    <footer class="block w-screen">
        <div class=" bg-gray-200">
            <div class="flex lg:flex-row flex-col lg:justify-between lg:items-start p-12">
                <div class=" col-md-6 border border-b-gray-400 border-y-2 lg:border-none">
                    <h5 class=" uppercase text-lg text-center font-normal">News-365</h5>
                    <p class="text-center">Here you can use rows and columns to organize your footer content.</p>
                </div>
                <div class="col-md-3">
                    <h5 class=" uppercase text-center text-lg  font-normal lg:mt-0 mt-3">LINKS</h5>
                    <ul class="text-center">
                        <li>
                            <NuxtLink class="text-blue-500 underline" to="#">Link 1</NuxtLink>
                        </li>
                        <li>
                            <NuxtLink class="text-blue-500 underline" to="#">Link 2</NuxtLink>
                        </li>
                        <li>
                            <NuxtLink class="text-blue-500 underline" to="#">Link 3</NuxtLink>
                        </li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <h5 class=" uppercase text-center font-normal text-lg lg:mt-0 mt-3">LINKS</h5>
                    <ul class="text-center">
                        <li>
                            <NuxtLink class="text-blue-500 underline" to="#">Link 1</NuxtLink>
                        </li>
                        <li>
                            <NuxtLink class="text-blue-500 underline" to="#">Link 2</NuxtLink>
                        </li>
                        <li>
                            <NuxtLink class="text-blue-500 underline" to="#">Link 3</NuxtLink>
                        </li>
                    </ul>
                </div>
                
            </div>
            <div class="text-black font-normal flex flex-row justify-center items-center text-center">
                    <h5 class=" font-medium">© 2022 Copyright:</h5>
                    <NuxtLink class="font-normal text-blue-500 underline" to="https://twitter.com/akham_gilbert">Gilbert Akham</NuxtLink>
                </div>
        </div>
    </footer>
</template>

<script setup>

</script>

<style lang="scss" scoped>

</style>