<template>
    <section class="bg-white w-screen h-screen">
        <div class="text-primary p-5">
            <h1 class="font-bold">Adventure Is Waiting</h1>
            <p class="font-extralight">Welcome, brave explorer! To embark on your next thrilling adventure.
            </p>
        </div>
        <section class="grid gap-12 pt-5 flex items-center justify-center">
            <div class="flex justify-center w-96">
                <select id="category"
                    class="w-4/5 border border-gray-300 text-gray-700 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block p-3 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500 bg-white shadow-sm appearance-none cursor-pointer"
                    required="">
                    <option value="" disabled selected hidden class="text-gray-400 ">Select category</option>
                    <option value="student" class="text-gray-700">Student</option>
                    <option value="alumni" class="text-gray-700">Alumni</option>
                    <option value="mentor" class="text-gray-700">Mentor</option>
                    <option value="visitor" class="text-gray-700">Visitor</option>
                </select>
            </div>
            <div class="flex justify-center w-96">
                <select id="category"
                    class="w-4/5 border border-gray-300 text-gray-700 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block p-3 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500 bg-white shadow-sm appearance-none cursor-pointer"
                    required="">
                    <option value="" disabled selected hidden class="text-gray-400 ">Department</option>
                    <option value="student" class="text-gray-700">Dept. Computer Application</option>
                    <option value="alumni" class="text-gray-700">Dept. Commerce</option>
                    <option value="mentor" class="text-gray-700">Dept. Psychology</option>
                    <option value="visitor" class="text-gray-700">Dept. Management</option>
                    <option value="visitor" class="text-gray-700">Dept. Geology</option>
                    <option value="visitor" class="text-gray-700">Dept. Social Work</option>
                </select>
            </div>
            <div class="flex justify-center w-96">
                <select id="category"
                    class="w-4/5 border border-gray-300 text-gray-700 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block p-3 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500 bg-white shadow-sm appearance-none cursor-pointer"
                    required="">
                    <option value="" disabled selected hidden class="text-gray-400 ">UG/PG</option>
                    <option value="student" class="text-gray-700">Under Graduation</option>
                    <option value="alumni" class="text-gray-700">Post Graduation</option>
                </select>
            </div>
            <div class="flex justify-center w-96">
                <input type="text" placeholder="Year of Admission" class="border-0 text-primary border-b-2 border-primary w-4/5 focus:outline-none focus:border-b-2 focus:ring-0 focus:border-primary">
            </div>
            <div>
                <h1 class="font-bold text-primary px-5">Your Skills</h1>
                <ButtonGroup />
            </div>
        </section>
        <div class="flex items-center justify-center ">
                <button type="button" class="flex absolute bottom-12   items-center justify-center text-white bg-primary hover:bg-gray-800 focus:outline-none focus:ring-4 focus:ring-gray-300 font-bold rounded-full w-4/5 py-5">Next</button>
            </div>

    </section>
</template>
<script>
import ButtonGroup from '../ButtonGroup.vue';

export default {
    name: 'signupStudent.vue',   
    components: {
        ButtonGroup,
    }
}
</script>