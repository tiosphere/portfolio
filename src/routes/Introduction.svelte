<script lang="ts">
	import { Briefcase, MapPin } from 'lucide-svelte';

	let { data } = $props();
</script>

<!--

    Coastal UI Design Basics:

    Main padding: 4
    Smaller alert / etc padding: 2
    border color: #222222
    card bg color: #0a0a0a
    rounded: lg

-->

<div class="w-full flex flex-col items-center justify-center">
	<div class="flex flex-col sm:flex-row items-center justify-between w-full">
		<div class="flex flex-col sm:flex-row items-center w-full">
			<img
				alt="avatar of Jonathan"
				src={data.avatar}
				class="sm:h-16 sm:w-16 w-24 h-24 rounded-full shadow-lg shadow-background-secondary mb-2 sm:mb-0"
			/>
			<div class="flex flex-col items-center sm:items-start sm:ml-4 w-full">
				<div class="text-primary text-3xl">{data.name}</div>
				<div class="flex gap-4 text-faint text-sm sm:-mt-[2px]">
					<div class="flex gap-1 items-center"><Briefcase size={14} />{data.occupation}</div>
					<div class="flex gap-1 items-center"><MapPin size={14} />{data.location}</div>
				</div>
			</div>
		</div>
		<div class="flex items-center space-x-5 sm:space-x-3 mt-6 sm:mt-2">
			<a
				aria-label="send an email"
				href={data.socials.email}
				target="_blank"
				class="cursor-pointer"
			>
				<svg class="h-11 w-11 sm:h-6 sm:w-6 text-faint hover:text-secondary" viewBox="0 0 24 24"
					><path
						fill="currentColor"
						d="M20 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2m0 4l-8 5l-8-5V6l8 5l8-5z"
					/></svg
				>
			</a>
			<div class="h-5 sm:h-3.5 w-[1px] bg-faint/50"></div>
			<a
				aria-label="LinkedIn Social Media link"
				href={data.socials.linkedin}
				target="_blank"
				class="cursor-pointer"
			>
				<svg class="h-11 w-11 sm:h-6 sm:w-6 text-faint hover:text-secondary" viewBox="0 0 1024 1024"
					><path
						fill="currentColor"
						d="M880 112H144c-17.7 0-32 14.3-32 32v736c0 17.7 14.3 32 32 32h736c17.7 0 32-14.3 32-32V144c0-17.7-14.3-32-32-32M349.3 793.7H230.6V411.9h118.7zm-59.3-434a68.8 68.8 0 1 1 68.8-68.8c-.1 38-30.9 68.8-68.8 68.8m503.7 434H675.1V608c0-44.3-.8-101.2-61.7-101.2c-61.7 0-71.2 48.2-71.2 98v188.9H423.7V411.9h113.8v52.2h1.6c15.8-30 54.5-61.7 112.3-61.7c120.2 0 142.3 79.1 142.3 181.9z"
					/></svg
				>
			</a>
		</div>
	</div>
	<div id="aboutSection" class="flex flex-col justify-start w-full mt-16">
		<div class="text-faint text-xs font-extrabold uppercase">About</div>
		<div class="text-primary mt-3">{data.description}</div>
	</div>
</div>
