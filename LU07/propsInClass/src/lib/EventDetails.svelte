<script lang="ts">
  export let description: string = "";
  export let date: string = "";
  export let time: string = "";
  export let location: string = "";
  export let color: "blue" | "purple" | "emerald" | "rose" = "blue";

  const colorClasses = {
    blue: "border-blue-100 hover:border-blue-200 bg-blue-50 text-blue-700",
    purple: "border-purple-100 hover:border-purple-200 bg-purple-50 text-purple-700",
    emerald: "border-emerald-100 hover:border-emerald-200 bg-emerald-50 text-emerald-700",
    rose: "border-rose-100 hover:border-rose-200 bg-rose-50 text-rose-700"
  };
</script>

<div class="bg-white shadow-lg rounded-lg p-8 border transition-colors {colorClasses[color].split(' ')[0]} {colorClasses[color].split(' ')[1]}">
  <p class="text-gray-700 mb-8 text-lg leading-relaxed">{description}</p>
  <div class="space-y-4 p-6 rounded-lg {colorClasses[color].split(' ')[2]}">
    <div class="flex items-center group">
      <span class="font-semibold w-24 {colorClasses[color].split(' ')[3]}">Date:</span>
      <span class="text-gray-800 group-hover:{colorClasses[color].split(' ')[3]} transition-colors">{date}</span>
    </div>
    <div class="flex items-center group">
      <span class="font-semibold w-24 {colorClasses[color].split(' ')[3]}">Time:</span>
      <span class="text-gray-800 group-hover:{colorClasses[color].split(' ')[3]} transition-colors">{time}</span>
    </div>
    <div class="flex items-center group">
      <span class="font-semibold w-24 {colorClasses[color].split(' ')[3]}">Location:</span>
      <span class="text-gray-800 group-hover:{colorClasses[color].split(' ')[3]} transition-colors">{location}</span>
    </div>
  </div>
</div>
