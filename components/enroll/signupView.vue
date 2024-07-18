<template>
    <section class="bg-white w-screen h-screen">
        <div class="text-primary p-5">
            <h1 class="font-bold">Adventure Is Waiting</h1>
            <p class="font-extralight">Welcome, brave explorer! To embark on your next thrilling adventure.
            </p>
        </div>
        <div class="flex items-center justify-center">
            <img src="public/assets/Sign up-bro 1.png" alt="Logo" class="max-w-full max-h-full">
        </div>
        <section class="grid gap-12 pt-5">
            <div class="flex items-center justify-center">
                <input type="text" placeholder="First name" class="border-0 text-primary border-b-2 border-primary w-4/5 focus:outline-none focus:border-b-2 focus:ring-0 focus:border-primary" required>
            </div>
            <div class="flex items-center justify-center">
                <input type="text" placeholder="Last name" class="border-0 text-primary border-b-2 border-primary w-4/5 focus:outline-none focus:border-b-2 focus:ring-0 focus:border-primary" required>
            </div>
            <div class="flex items-center justify-center">
                <input type="text" placeholder="Email" class="border-0 text-primary border-b-2 border-primary w-4/5 focus:outline-none focus:border-b-2 focus:ring-0 focus:border-primary" required>
            </div>
            <div class="flex items-center justify-center">
                <input type="text" placeholder="Mobile" class="border-0 text-primary border-b-2 border-primary w-4/5 focus:outline-none focus:border-b-2 focus:ring-0 focus:border-primary" required>
            </div>
            <div class="flex items-center justify-center">
                <button type="button" class="flex items-center justify-center text-white bg-primary hover:bg-gray-800 focus:outline-none focus:ring-4 focus:ring-gray-300 font-bold rounded-full w-4/5 py-3">Next</button>
            </div>           
        </section>
        
    </section>
</template>
<script>
export default {
    name: 'signupView.vue',
}
</script>      