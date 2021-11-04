<template>
    <div class="bg-purple-400">
        <div class="container mx-auto flex items-center justify-between text-purple-50">
            <h1 class="tracking-tighter text-3xl font-thin">
                Basic<span class="font-semibold">Router</span>
            </h1>
            <nav>
                <ul class="flex space-x-4">
                    <router-link to="/">
                        <li class="py-5 px-4 hover:cursor-pointer hover:bg-purple-300">Home</li>
                    </router-link>
                    <router-link to="/about">
                        <li class="py-5 px-4 hover:cursor-pointer hover:bg-purple-300">About</li>
                    </router-link>
                    <router-link to="/hello">
                        <li class="py-5 px-4 hover:cursor-pointer hover:bg-purple-300">Hello</li>
                    </router-link>
                </ul>
            </nav>
        </div>
    </div>
</template>