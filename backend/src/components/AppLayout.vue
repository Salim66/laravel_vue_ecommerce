<template>
    <div class="min-h-full bg-gray-200 flex">
      <!--    Sidebar-->
      <Sidebar :class="{'-ml-[200px]': !sidebarOpened}"/>
      <!--/    Sidebar-->

      <div class="flex-1">
        <Navbar @toggle-sidebar="toggleSidebar"></Navbar>
        <!--      Content-->
        <main class="p-6">
          <router-view></router-view>
        </main>
        <!--      Content-->
      </div>
    </div>
    <!-- <div v-else class="min-h-full bg-gray-200 flex items-center justify-center">
      <Spinner />
    </div> -->
</template>

<script setup>
    import Sidebar from "./Sidebar.vue";
    import Navbar from "./Navbar.vue";
    import store from "../store";

    const {title} = defineProps({
    title: String
    })
</script>

<style scoped>

</style>
