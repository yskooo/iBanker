<template>
  <aside>
    <div
      class="flex h-full w-full flex-col gap-5 overflow-y-auto rounded-md border bg-card pb-5 scrollbar-thin scrollbar-thumb-input scrollbar-thumb-rounded-md"
    >
      <SidebarItem :links="menu" />

      <div class="mt-auto">
        <SidebarItem :links="bottomMenu" />
      </div>
    </div>
  </aside>
</template>

<script setup lang="ts">
  const bottomMenu = [
    {
      title: "Settings",
      icon: "heroicons:cog-8-tooth",
    },
    {
      title: "Logout",
      icon: "heroicons:arrow-left-on-rectangle",
    },
  ];
  const menu = [
    {
      title: "Dashboard",
      icon: "heroicons:home",
    },
    {
      title: "Investors",
      icon: "heroicons:user-group",
      items: [
      
      ],
    },

    {
      title: "Products",
      icon: "heroicons:cube",
      items: [

      ],
    },
    {
      title: "Staff",
      icon: "heroicons:user",
      items: [
       
      ],
    },
    {
      title: "Analytics",
      icon: "heroicons:chart-pie",
      items: [{ title: "Overview" }, { title: "Statistics" }, { title: "Trends" }],
    },
  ];
</script>
