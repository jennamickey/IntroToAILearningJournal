<script lang="ts">
  export let eventName: string = "Event Name Here";
  export let color: "blue" | "purple" | "emerald" | "rose" = "blue";

  const colorClasses = {
    blue: "text-blue-600 border-blue-200 hover:text-blue-700",
    purple: "text-purple-600 border-purple-200 hover:text-purple-700",
    emerald: "text-emerald-600 border-emerald-200 hover:text-emerald-700",
    rose: "text-rose-600 border-rose-200 hover:text-rose-700"
  };
</script>

<h1 class="text-4xl font-bold mb-6 py-2 border-b-2 transition-colors {colorClasses[color]}">{eventName}</h1>
