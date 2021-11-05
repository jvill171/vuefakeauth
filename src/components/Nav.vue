<template>
    <div class="bg-red-400">
        <div class="container mx-auto flex items-center justify-between text-red-50">
            <h1 class="tracking-tighter text-3xl font-thin">
                Vue<span class="font-semibold">FakeAuth</span>
            </h1>
            <nav>
                <ul class="flex space-x-4">
                    <router-link to="/">
                        <li class="py-5 px-4 hover:cursor-pointer hover:bg-red-300">Home</li>
                    </router-link>
                    <router-link to="/about">
                        <li class="py-5 px-4 hover:cursor-pointer hover:bg-red-300">About</li>
                    </router-link>
                    <router-link to="/login">
                        <li class="py-5 px-4 hover:cursor-pointer hover:bg-red-300">Login</li>
                    </router-link>
                </ul>
            </nav>
        </div>
    </div>
</template>