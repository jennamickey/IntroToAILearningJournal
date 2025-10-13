
<script lang="ts">
	import Header from '$lib/Header.svelte';
	import EventDetails from '$lib/EventDetails.svelte';
</script>

<main class="flex items-center justify-center min-h-screen bg-gradient-to-b from-gray-50 to-gray-100 p-8">
	<div class="max-w-3xl w-full space-y-12">
		<div>
			<Header eventName="Iowa Tech Summit" color="blue" />
			<EventDetails
				description="Connect, learn, and grow at Iowa's premier technology conference"
				date="September 15, 2025"
				time="10:00 AM"
				location="Iowa Event Center"
				color="blue"
			/>
		</div>

		<div>
			<Header eventName="Des Moines Web Dev Meetup" color="purple" />
			<EventDetails
				description="Join local developers for an evening of networking, lightning talks, and hands-on coding workshops focused on modern web development"
				date="October 20, 2025"
				time="6:30 PM"
				location="Franklin Junior High Event Center"
				color="purple"
			/>
		</div>
	</div>
</main>
