<template>
<!-- component -->
<!-- Root element for center items -->
<div class="flex flex-col h-screen bg-gray-100 ">
    <!-- Auth Card Container -->
    <div class="grid place-items-center mx-2 my-20 sm:my-auto">
        <!-- Auth Card -->
        <div class="w-11/12 p-12 sm:w-8/12 md:w-6/12 lg:w-5/12 2xl:w-4/12 
            px-6 py-10 sm:px-10 sm:py-6 
            bg-white rounded-lg shadow-md lg:shadow-lg">

            <!-- Card Title -->
            <h2 class="text-center font-semibold text-3xl lg:text-4xl text-gray-800">
                Login
            </h2>

            <form class="mt-10" >
                <!-- Email Input -->
                <label for="email" class="mb-2 block text-xs font-semibold text-gray-600 uppercase">E-mail</label>
                <q-input outlined :dense="dense" class="mb-2 "/>

                <!-- Password Input -->
                <label for="password" class="block mt-2 mb-2 text-xs font-semibold text-gray-600 uppercase"
                >Password</label>
                <q-input outlined :dense="dense" class="mb-2" type="password"/>

                <!-- Auth Buttton -->
               <q-btn label="Login"  class="full-width" color="grey-7"></q-btn>

                <!-- Another Auth Routes -->
                <div class="sm:flex sm:flex-wrap mt-8 sm:mb-4 text-sm text-center">
                    <a href="forgot-password" class="flex-2 underline">
                        Forgot password?
                    </a>

                    <p class="flex-1 text-gray-500 text-md mx-4 my-1 sm:my-auto">
                        or
                    </p>
        
                    <a href="register" class="flex-2 underline">
                        Create an Account
                    </a>
                </div>
            </form>
        </div>
    </div>
</div>

</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class HelloWorld extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
