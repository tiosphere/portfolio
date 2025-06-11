<script lang="ts">
	import Introduction from './Introduction.svelte';
	import Experience from './Experience.svelte';
	import Education from './Education.svelte';
	import Skills from './Skills.svelte';
	import PersonalProjects from './PersonalProjects.svelte';

	const portfolioContent: any = {
		introduction: {
			name: 'Chiraphat Lua',
			occupation: 'SaaS Enthusiast',
			location: 'Bangkok, Thailand',
			description:
				"A Software Engineer, I'm passionate about building SaaS products that solve real-world problems. With a focus on user experience and performance, I strive to create applications that are not only functional but also delightful to use.",
			avatar: 'https://avatars.githubusercontent.com/u/107175519?s=400&v=4',
			socials: {
				email: 'mailto:chiraphat.lua@clua.top',
				linkedin: 'https://www.linkedin.com/in/chiraphat-lua/'
			}
		},
		experiences: [
			{
				company: 'Agoda',
				role: 'Software Engineer Intern',
				duration: 'Aug. 2024 to Mar. 2025',
				image:
					'https://cdn.brandfetch.io/idrJbkwvG0/w/400/h/400/theme/dark/icon.jpeg?c=1dxbfHSJFAPEGdCLU4o5B'
			}
		],
		education: {
			image: 'https://muic.mahidol.ac.th/eng/wp-content/downloads/CI/logo_2021/MU_Logo.png',
			school: 'Mahidol University International College',
			degree: 'Bachelor of Science in Computer Science',
			graduationYear: '2025'
		},
		skills: [
			{
				icon: `<svg class="h-4 w-4 text-primary" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path fill="currentColor" d="M19.8 3.77a6.25 6.25 0 0 0-8.63-1.913L6.11 5.081a6.25 6.25 0 0 0-1.973 8.532a6.25 6.25 0 0 0 8.693 8.53l5.06-3.224a6.25 6.25 0 0 0 1.974-8.532A6.25 6.25 0 0 0 19.8 3.77m-1.352 5.004A6.26 6.26 0 0 0 15.65 7.5a1 1 0 0 0-1.525-1.003L9.066 9.72a1 1 0 1 0 1.075 1.686l2.109-1.343a4.25 4.25 0 1 1 4.567 7.17l-5.06 3.223a4.25 4.25 0 0 1-6.203-5.23A6.25 6.25 0 0 0 8.35 16.5a1 1 0 0 0 1.525 1.003l5.06-3.224a1 1 0 0 0-1.074-1.687l-2.109 1.344a4.25 4.25 0 0 1-4.567-7.17l5.06-3.223a4.25 4.25 0 0 1 6.203 5.23"/></svg>`,
				text: 'Svelte'
			},
			{
				icon: `<svg class="h-4 w-4 text-primary" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path fill="currentColor" d="M12 2A10 10 0 0 0 2 12c0 4.42 2.87 8.17 6.84 9.5c.5.08.66-.23.66-.5v-1.69c-2.77.6-3.36-1.34-3.36-1.34c-.46-1.16-1.11-1.47-1.11-1.47c-.91-.62.07-.6.07-.6c1 .07 1.53 1.03 1.53 1.03c.87 1.52 2.34 1.07 2.91.83c.09-.65.35-1.09.63-1.34c-2.22-.25-4.55-1.11-4.55-4.92c0-1.11.38-2 1.03-2.71c-.1-.25-.45-1.29.1-2.64c0 0 .84-.27 2.75 1.02c.79-.22 1.65-.33 2.5-.33s1.71.11 2.5.33c1.91-1.29 2.75-1.02 2.75-1.02c.55 1.35.2 2.39.1 2.64c.65.71 1.03 1.6 1.03 2.71c0 3.82-2.34 4.66-4.57 4.91c.36.31.69.92.69 1.85V21c0 .27.16.59.67.5C19.14 20.16 22 16.42 22 12A10 10 0 0 0 12 2"/></svg>`,
				text: 'Github'
			},
			{
				icon: `<svg class="h-4 w-4 text-primary" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path fill="currentColor" d="M12 10.11c1.03 0 1.87.84 1.87 1.89c0 1-.84 1.85-1.87 1.85S10.13 13 10.13 12c0-1.05.84-1.89 1.87-1.89M7.37 20c.63.38 2.01-.2 3.6-1.7c-.52-.59-1.03-1.23-1.51-1.9a23 23 0 0 1-2.4-.36c-.51 2.14-.32 3.61.31 3.96m.71-5.74l-.29-.51c-.11.29-.22.58-.29.86c.27.06.57.11.88.16zm6.54-.76l.81-1.5l-.81-1.5c-.3-.53-.62-1-.91-1.47C13.17 9 12.6 9 12 9s-1.17 0-1.71.03c-.29.47-.61.94-.91 1.47L8.57 12l.81 1.5c.3.53.62 1 .91 1.47c.54.03 1.11.03 1.71.03s1.17 0 1.71-.03c.29-.47.61-.94.91-1.47M12 6.78c-.19.22-.39.45-.59.72h1.18c-.2-.27-.4-.5-.59-.72m0 10.44c.19-.22.39-.45.59-.72h-1.18c.2.27.4.5.59.72M16.62 4c-.62-.38-2 .2-3.59 1.7c.52.59 1.03 1.23 1.51 1.9c.82.08 1.63.2 2.4.36c.51-2.14.32-3.61-.32-3.96m-.7 5.74l.29.51c.11-.29.22-.58.29-.86c-.27-.06-.57-.11-.88-.16zm1.45-7.05c1.47.84 1.63 3.05 1.01 5.63c2.54.75 4.37 1.99 4.37 3.68s-1.83 2.93-4.37 3.68c.62 2.58.46 4.79-1.01 5.63c-1.46.84-3.45-.12-5.37-1.95c-1.92 1.83-3.91 2.79-5.38 1.95c-1.46-.84-1.62-3.05-1-5.63c-2.54-.75-4.37-1.99-4.37-3.68s1.83-2.93 4.37-3.68c-.62-2.58-.46-4.79 1-5.63c1.47-.84 3.46.12 5.38 1.95c1.92-1.83 3.91-2.79 5.37-1.95M17.08 12c.34.75.64 1.5.89 2.26c2.1-.63 3.28-1.53 3.28-2.26s-1.18-1.63-3.28-2.26c-.25.76-.55 1.51-.89 2.26M6.92 12c-.34-.75-.64-1.5-.89-2.26c-2.1.63-3.28 1.53-3.28 2.26s1.18 1.63 3.28 2.26c.25-.76.55-1.51.89-2.26m9 2.26l-.3.51c.31-.05.61-.1.88-.16c-.07-.28-.18-.57-.29-.86zm-2.89 4.04c1.59 1.5 2.97 2.08 3.59 1.7c.64-.35.83-1.82.32-3.96c-.77.16-1.58.28-2.4.36c-.48.67-.99 1.31-1.51 1.9M8.08 9.74l.3-.51c-.31.05-.61.1-.88.16c.07.28.18.57.29.86zm2.89-4.04C9.38 4.2 8 3.62 7.37 4c-.63.35-.82 1.82-.31 3.96a23 23 0 0 1 2.4-.36c.48-.67.99-1.31 1.51-1.9"/></svg>`,
				text: 'React'
			},
			{
				icon: `<svg class="h-4 w-4 text-primary" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path fill="currentColor" d="M3 3v18h18V3zm9.813 14.023c0 1.77-1.045 2.584-2.555 2.584c-1.335 0-2.12-.697-2.526-1.568l1.394-.871c.232.493.493.87 1.103.87c.58 0 .9-.203.9-1.073v-5.69h1.684zm4.006 2.584c-1.567 0-2.583-.784-3.106-1.713l1.394-.813c.377.58.87 1.016 1.683 1.016c.697 0 1.133-.32 1.133-.871c0-.58-.436-.784-1.22-1.133l-.406-.174c-1.22-.493-2.033-1.19-2.033-2.584c0-1.277.93-2.206 2.468-2.206c1.075 0 1.83.378 2.38 1.364l-1.305.871c-.29-.493-.581-.725-1.104-.725c-.493 0-.813.32-.813.726c0 .493.32.696 1.017 1.016l.406.174c1.422.61 2.264 1.22 2.264 2.67c.03 1.54-1.16 2.381-2.758 2.381"/></svg>`,
				text: 'JavaScript'
			},
			{
				icon: `<svg class="h-4 w-4 text-primary" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path fill="currentColor" d="M19.131 3H4.869c-.955 0-1.73.787-1.73 1.758v14.484c0 .97.775 1.758 1.73 1.758h14.262c.956 0 1.73-.787 1.73-1.758V4.758c0-.97-.774-1.758-1.73-1.758m-5.712 9.984h-2.215v6.434H9.439v-6.434H7.223v-1.441h6.196zm5.712 5.277c-.139.317-.377.552-.658.739a3 3 0 0 1-.969.386a5.6 5.6 0 0 1-1.177.12a6.5 6.5 0 0 1-1.211-.11a3.7 3.7 0 0 1-1.004-.33v-1.689l-.066-.053l.066-.015v.068q.441.357.972.545c.347.133.727.2 1.108.2c.242 0 .426-.021.589-.06a1.4 1.4 0 0 0 .415-.168a.7.7 0 0 0 .246-.253a.7.7 0 0 0-.052-.738a1.3 1.3 0 0 0-.346-.335a3 3 0 0 0-.52-.295c-.207-.095-.418-.194-.657-.292c-.589-.281-1.053-.562-1.35-.95c-.301-.35-.45-.808-.45-1.335c0-.422.08-.76.242-1.055c.173-.316.377-.548.658-.738c.277-.193.588-.334.969-.422c.38-.088.762-.133 1.177-.133s.762.024 1.073.073c.311.05.602.127.865.229v1.652a2.3 2.3 0 0 0-.415-.242a3.8 3.8 0 0 0-.97-.275a3 3 0 0 0-.45-.033a2.4 2.4 0 0 0-.553.057a1.3 1.3 0 0 0-.416.161a.8.8 0 0 0-.26.25a.6.6 0 0 0-.093.327q0 .194.104.351q.103.152.295.296c.114.091.27.183.45.274c.207.091.394.183.623.278c.311.133.588.281.83.422c.243.14.447.305.623.492c.187.175.322.387.416.633s.142.523.142.843c0 .457-.108.809-.246 1.125"/></svg>`,
				text: 'TypeScript'
			},
			{
				icon: `<svg class="h-4 w-4 text-primary" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path fill="currentColor" d="M19.14 7.5A2.86 2.86 0 0 1 22 10.36v3.78A2.86 2.86 0 0 1 19.14 17H12c0 .39.32.96.71.96H17v1.68a2.86 2.86 0 0 1-2.86 2.86H9.86A2.86 2.86 0 0 1 7 19.64v-3.75a2.85 2.85 0 0 1 2.86-2.85h5.25a2.85 2.85 0 0 0 2.85-2.86V7.5zm-4.28 11.79c-.4 0-.72.3-.72.89s.32.71.72.71a.71.71 0 0 0 .71-.71c0-.59-.32-.89-.71-.89m-10-1.79A2.86 2.86 0 0 1 2 14.64v-3.78A2.86 2.86 0 0 1 4.86 8H12c0-.39-.32-.96-.71-.96H7V5.36A2.86 2.86 0 0 1 9.86 2.5h4.28A2.86 2.86 0 0 1 17 5.36v3.75a2.85 2.85 0 0 1-2.86 2.85H8.89a2.85 2.85 0 0 0-2.85 2.86v2.68zM9.14 5.71c.4 0 .72-.3.72-.89s-.32-.71-.72-.71c-.39 0-.71.12-.71.71s.32.89.71.89"/></svg>`,
				text: 'Python'
			},
			{
				icon: `<svg class="h-4 w-4 text-primary" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"><path fill="currentColor" d="M 17.625 3 C 19.027344 6.308594 12.597656 8.335938 12 11.09375 C 11.453125 13.625 15.808594 16.59375 15.8125 16.59375 C 15.148438 15.546875 14.664063 14.664063 14 13.03125 C 12.875 10.273438 20.855469 7.785156 17.625 3 Z M 21.875 7.59375 C 21.875 7.59375 16.253906 7.949219 15.96875 11.625 C 15.839844 13.261719 17.453125 14.121094 17.5 15.3125 C 17.539063 16.285156 16.53125 17.09375 16.53125 17.09375 C 16.53125 17.09375 18.339844 16.765625 18.90625 15.28125 C 19.53125 13.632813 17.6875 12.507813 17.875 11.1875 C 18.054688 9.925781 21.875 7.59375 21.875 7.59375 Z M 23.25 16.0625 C 22.660156 16.035156 21.996094 16.253906 21.40625 16.6875 C 22.570313 16.429688 23.5625 17.160156 23.5625 18 C 23.5625 19.882813 20.875 21.65625 20.875 21.65625 C 20.875 21.65625 25.03125 21.191406 25.03125 18.09375 C 25.03125 16.816406 24.230469 16.109375 23.25 16.0625 Z M 12.21875 16.09375 C 10.769531 16.144531 7.875 16.382813 7.875 17.5 C 7.875 19.054688 14.617188 19.175781 19.4375 18.21875 C 19.4375 18.21875 20.75 17.304688 21.09375 16.96875 C 17.933594 17.625 10.71875 17.726563 10.71875 17.15625 C 10.71875 16.632813 13.03125 16.09375 13.03125 16.09375 C 13.03125 16.09375 12.703125 16.078125 12.21875 16.09375 Z M 11.78125 18.96875 C 10.988281 18.96875 9.8125 19.585938 9.8125 20.1875 C 9.8125 21.398438 15.78125 22.328125 20.1875 20.5625 L 18.65625 19.625 C 15.667969 20.601563 10.148438 20.277344 11.78125 18.96875 Z M 12.53125 21.6875 C 11.449219 21.6875 10.75 22.371094 10.75 22.875 C 10.75 24.425781 17.214844 24.578125 19.78125 23 L 18.15625 21.9375 C 16.242188 22.761719 11.425781 22.882813 12.53125 21.6875 Z M 8.90625 23.09375 C 7.140625 23.058594 6 23.859375 6 24.53125 C 6 28.105469 24.09375 27.933594 24.09375 24.28125 C 24.09375 23.675781 23.378906 23.386719 23.125 23.25 C 24.601563 26.742188 8.34375 26.46875 8.34375 24.40625 C 8.34375 23.9375 9.546875 23.46875 10.65625 23.6875 L 9.71875 23.15625 C 9.441406 23.113281 9.160156 23.097656 8.90625 23.09375 Z M 26 25.5 C 23.25 28.160156 16.289063 29.113281 9.28125 27.46875 C 16.289063 30.398438 25.964844 28.769531 26 25.5 Z"></path></g></svg>`,
				text: 'Java'
			},
			{
				icon: `<svg class="h-4 w-4 text-primary" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"><title>Scala icon</title><path fill="currentColor" d="M4.589 24c4.537 0 13.81-1.516 14.821-3v-5.729c-.957 1.408-10.284 2.912-14.821 2.912V24zM4.589 16.365c4.537 0 13.81-1.516 14.821-3V7.636c-.957 1.408-10.284 2.912-14.821 2.912v5.817zM4.589 8.729c4.537 0 13.81-1.516 14.821-3V0C18.453 1.408 9.126 2.912 4.589 2.912v5.817z"></path></g></svg>`,
				text: 'Scala'
			}
		],
		projects: [
			{
				name: 'Anime Streaming Demo',
				technology: 'Django',
				description:
					'Online anime streaming demo website built with Django and plain CSS/JS. It is a simple anime streaming website that can be used to watch anime online.',
				image: 'anime-demo-preview.png',
				link: 'https://anime-demo.clua.top/'
			},
			{
				name: 'JustCalculator Website',
				technology: 'Svelte',
				description:
					'Basic calculator website built with Svelte 5 and host on Cloudflare Page. It is a simple calculator that can be used for basic arithmetic operations.',
				image: 'justcalculator-preview.png',
				link: 'https://justcalculator.net/'
			},
			{
				name: 'String Length Calculator',
				technology: 'Svelte',
				description:
					'Online tool to calculate the length of a string. It is built with Svelte 5 and host on Cloudflare Page. It can be used to calculate the length of a string in various formats.',
				image: 'stringlengthonline-preview.png',
				link: 'https://stringlengthonline.com/'
			}
		]
	};
</script>

<div class="overflow-x-hidden bg-background flex flex-col justify-center items-center relative">
	<div class="w-full max-w-[680px] flex flex-col my-24 lg:px-0 px-5 mb-[100px] sm:mb-[200px]">
		<Introduction data={portfolioContent.introduction} />
		<Experience data={portfolioContent.experiences} />
		<Education data={portfolioContent.education} />
		<Skills data={portfolioContent.skills} />
		<div
			class="w-full h-[1px] bg-gradient-to-r from-zinc-900 to-zinc-900 via-zinc-800 my-12 mb-16"
		></div>
		<div class="mb-4 flex flex-col items-center">
			<div class="text-3xl text-primary font-bold">My Work</div>
			<div class="text-faint font-thin mt-1">Collected across various projects.</div>
		</div>
		<PersonalProjects data={portfolioContent.projects} />
	</div>
	<div
		class="bg-gradient-to-b from-background to-background-secondary bg-background h-[200px] w-full"
	></div>
</div>
