
<template>
    <GuestLayout title="Set new password">
        <form class="mt-8 space-y-6" action="#" method="POST">
          <input type="hidden" name="remember" value="true" />
          <div class="-space-y-px rounded-md shadow-sm">
            <div>
              <label for="password" class="sr-only">New Password</label>
              <input id="password" name="password" type="password" autocomplete="current-password" required="" class="relative block w-full appearance-none rounded-none rounded-b-md border border-gray-300 px-3 py-2 text-gray-900 placeholder-gray-500 focus:z-10 focus:border-indigo-500 focus:outline-none focus:ring-indigo-500 sm:text-sm" placeholder="New Password" />
            </div>
            <div>
              <label for="password" class="sr-only">Repeat Password</label>
              <input id="password" name="password" type="password" autocomplete="current-password" required="" class="relative block w-full appearance-none rounded-none rounded-b-md border border-gray-300 px-3 py-2 text-gray-900 placeholder-gray-500 focus:z-10 focus:border-indigo-500 focus:outline-none focus:ring-indigo-500 sm:text-sm" placeholder="Repeat Password" />
            </div>
          </div>

          <div class="flex items-center justify-between">
            <div class="text-sm">
              <router-link :to="{ name: 'login' }" class="font-medium text-indigo-600 hover:text-indigo-500">Go back to login</router-link>
            </div>
          </div>

          <div>
            <button type="submit" class="group relative flex w-full justify-center rounded-md border border-transparent bg-indigo-600 py-2 px-4 text-sm font-medium text-white hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:ring-offset-2">
              Submit
            </button>
          </div>
        </form>
    </GuestLayout>
</template>

<script setup>
import GuestLayout from '../components/GuestLayout.vue';
</script>

<style>

</style>
