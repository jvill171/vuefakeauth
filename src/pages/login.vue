<script setup>
import {ref} from "vue";
import {useRouter} from "vue-router";
import useAuth from "../composable/useAuth";

const { isAuthenticated, login } = useAuth();

const username = ref("");
const password = ref("");

const router = useRouter();

const loginIn = () => {
    login(username.value, password.value);
    if(isAuthenticated.value){
        router.push("/");
    }
};
</script>

<template >
<div class="flex-col space-y-12 flex items-center justify-center min-h-screen-nonav">
    Logged in: {{isAuthenticated}}
    <div class="bg-gray-200 flex justify-center items-center shadow-2xl overflow-hidden rounded-lg">
        <img class="h-64" src="../assets/bg_login.png" alt="Login BG">
        <form @submit.prevent="loginIn" class="flex flex-col space-y-4 p-4">
            <input type="text" class="p-2 border-2 rounded-lg" placeholder="Username" 
                v-model="username"/>
            <input type="password" class="p-2 border-2 rounded-lg" placeholder="Password" 
                v-model="password"/>
            <button @submit.prevent="loginIn" type="submit" class="py-2 rounded-lg bg-red-400 text-red-50">Login</button>
        </form>
    </div>
</div>
</template>