<template>
  <div class="sticky top-20 mt-5">
    <p class="font-bold">Reminders</p>

    <ul>
      <template v-for="(r, i) in reminders" :key="i">
        <li>
          <div class="mt-5 flex items-center justify-between">
            <div class="flex items-center gap-3">
              <Icon name="heroicons:check-circle" class="h-4 w-4 text-muted-foreground" />
              <span class="text-sm">{{ r.title }}</span>
            </div>
            <span class="text-sm text-muted-foreground">{{ r.time }}</span>
          </div>
        </li>
      </template>
    </ul>
  </div>
</template>

<script setup lang="ts">
  const reminders = [
    { title: "Meet Madrid", time: "10:00 AM" },
    { title: "Meet Jane", time: "11:00 AM" },
    { title: "Call Elon", time: "12:00 PM" },
    { title: "Power Nap", time: "1:00 PM" },
    { title: "Back to Work", time: "1:30 PM" },
  ];
</script>
