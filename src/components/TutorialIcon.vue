<template>
  <span @mousemove="fire" @mouseleave="bomb">{{ icon }}</span>
</template>

<script>
export default {
  data() {
    return {
      icon: "🧨",
    }
  },
  methods: {
    fire() {
      this.icon = "🔥"
    },
    bomb() {
      this.icon = "🧨"
    },
  },
}
</script>
