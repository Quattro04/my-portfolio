<template>
    <div class="h-screen flex">
        <SideMenu :opened="opened" />
        <SideMenuButton onChange="(val) => this.opened = val" />
        <div class="flex-1 flex flex-col lg:ml-60 bg-sky-100 rounded-l-3xl py-14 px-4 drop-shadow overflow-auto">
            <NuxtPage />
        </div>
    </div>
</template>
<script setup>
    useHead({
        link: [
            { href: 'https://fonts.googleapis.com', rel: 'preconnect' },
            { href: 'https://fonts.gstatic.com', rel: 'preconnect', crossorigin: true },
            { href: 'https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;700&family=Varela+Round&display=swap', rel: 'stylesheet' },
        ],
    });
</script>

<script>
    data: () => {
      return {
          opened: false
      };
    }
</script>
