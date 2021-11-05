<script setup></script>

<template >
<div class="flex-col space-y-12 flex items-center justify-center min-h-screen-nonav">
    <div class="bg-gray-200 flex justify-center items-center shadow-2xl overflow-hidden rounded-lg">
        <img class="h-64" src="../assets/bg_login.png" alt="Login BG">
        <form class="flex flex-col space-y-4 p-4">
            <input type="text" class="p-2 border-2 rounded-lg" placeholder="Username" />
            <input type="password" class="p-2 border-2 rounded-lg" placeholder="Password" />
            <button type="submit" class="py-2 rounded-lg bg-red-400 text-red-50">Login</button>
        </form>
    </div>
</div>
</template>