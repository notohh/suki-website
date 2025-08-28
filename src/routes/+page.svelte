<script>
	import Banner from '$lib/assets/banner.png'
	import Pfp from '$lib/assets/pfp.png'
	import Twitch from '$lib/components/Twitch.svelte'
	import Youtube from '$lib/components/Youtube.svelte'
	import Kofi from '$lib/components/Kofi.svelte'
	import Tiktok from '$lib/components/Tiktok.svelte'
	import X from '$lib/components/X.svelte'
	import Throne from '$lib/components/Throne.svelte'
	import Discord from '$lib/components/Discord.svelte'
	import GSupps from '$lib/components/GSupps.svelte'
	import Bed from '$lib/components/Bed.svelte'
</script>

<svelte:head>
	<title>suki</title>
</svelte:head>

<div class="relative">
	<!-- angled background -->
	<div
		class="clip-diagonal fixed top-0 left-0 -z-10 hidden sm:block"
		style="
      width: 100vw;
      height: 45rem;
      background-image: url('{Banner}');
      background-size: cover;
      background-repeat: no-repeat;
      background-position: center top;
      transform: translateZ(0);
      will-change: transform;
    "
	></div>

	<!-- gradient -->
	<div
		class="clip-diagonal fixed top-0 left-0 -z-10 hidden bg-gradient-to-b from-transparent to-base-100 sm:block"
		style="
      width: 100vw;
      height: 45rem;
      transform: translateZ(0);
      will-change: transform;
    "
	></div>
</div>

<div
	class="bg-base relative z-10 flex min-h-screen flex-col items-center justify-center font-display text-base-content"
>
	<img
		src={Pfp}
		alt="Sukivt model"
		class="pointer-events-none mb-4 ml-2 h-32 w-32 rounded-full"
	/>
	<div class="flex w-full flex-col items-center">
		<div
			class="pointer-events-none divider mx-auto w-80 divider-primary text-3xl font-medium md:w-128 lg:w-200"
		>
			suki
		</div>
		<div class="mt-4 grid grid-cols-1 gap-3 sm:grid-cols-3">
			<!-- Twitch -->
			<a
				href="https://www.twitch.tv/suki"
				class="card card-side w-full motion-preset-slide-right bg-black shadow-sm hover:bg-base-300"
			>
				<figure
					class="flex flex-shrink-0 items-center justify-center rounded-md bg-twitch-purple p-2"
				>
					<Twitch className="w-8 h-8 fill-white" />
				</figure>
				<div class="card-body min-w-0">
					<h2 class="pointer-events-none card-title">Twitch</h2>
					<div class="card-actions justify-end"></div>
				</div>
			</a>

			<!-- Youtube -->

			<a
				href="https://www.youtube.com/@sukiivt"
				class="card card-side w-full motion-preset-slide-right bg-black shadow-sm motion-delay-200 hover:bg-base-300"
			>
				<figure
					class="flex flex-shrink-0 items-center justify-center rounded-md bg-youtube-red p-2"
				>
					<Youtube className="w-8 h-8 fill-white" />
				</figure>
				<div class="card-body min-w-0">
					<h2 class="pointer-events-none card-title">Youtube</h2>
					<div class="card-actions justify-end"></div>
				</div>
			</a>

			<!-- ASMR -->

			<a
				href="https://www.youtube.com/@ASMRRSuki"
				class="card card-side w-full motion-preset-slide-right bg-black shadow-sm motion-delay-400 hover:bg-base-300"
			>
				<figure
					class="flex flex-shrink-0 items-center justify-center rounded-md bg-pink-400 p-2"
				>
					<Bed className="w-8 h-8" />
				</figure>
				<div class="card-body min-w-0">
					<h2 class="pointer-events-none card-title">ASMR</h2>
					<div class="card-actions justify-end"></div>
				</div>
			</a>

			<!-- Discord -->

			<a
				href="https://discord.gg/ssuki"
				class="card card-side w-full motion-preset-slide-right bg-black shadow-sm motion-delay-600 hover:bg-base-300"
			>
				<figure
					class="flex flex-shrink-0 items-center justify-center rounded-md bg-discord-purple p-2"
				>
					<Discord className="w-8 h-8 fill-white" />
				</figure>
				<div class="card-body min-w-0">
					<h2 class="pointer-events-none card-title">Discord</h2>
					<div class="card-actions justify-end"></div>
				</div>
			</a>

			<!-- X -->

			<a
				href="https://x.com/SukiiVT"
				class="card card-side w-full motion-preset-slide-right bg-black shadow-sm motion-delay-800 hover:bg-base-300"
			>
				<figure
					class="flex flex-shrink-0 items-center justify-center rounded-md bg-black p-2"
				>
					<X className="w-8 h-8 fill-white" />
				</figure>
				<div class="card-body min-w-0">
					<h2 class="pointer-events-none card-title">X</h2>
					<div class="card-actions justify-end"></div>
				</div>
			</a>

			<!-- Tiktok -->

			<a
				href="https://www.tiktok.com/@sukkivt"
				class="card card-side w-full motion-preset-slide-right bg-black shadow-sm motion-delay-1000 hover:bg-base-300"
			>
				<figure
					class="flex flex-shrink-0 items-center justify-center rounded-md bg-black p-2"
				>
					<Tiktok className="w-8 h-8 fill-white" />
				</figure>
				<div class="card-body min-w-0">
					<h2 class="pointer-events-none card-title">Tiktok</h2>
					<div class="card-actions justify-end"></div>
				</div>
			</a>

			<!-- Kofi -->

			<a
				href="https://ko-fi.com/sssuukiii"
				class="card card-side w-full motion-preset-slide-right bg-black shadow-sm motion-delay-1200 hover:bg-base-300"
			>
				<figure
					class="flex flex-shrink-0 items-center justify-center rounded-md bg-blue-500 p-2"
				>
					<Kofi className="w-8 h-8 fill-white" />
				</figure>
				<div class="card-body min-w-0">
					<h2 class="pointer-events-none card-title">Kofi</h2>
					<div class="card-actions justify-end"></div>
				</div>
			</a>

			<!-- Gamersupps -->

			<a
				href="https://gamersupps.gg/?ref=SUKI"
				class="card card-side w-full motion-preset-slide-right bg-black shadow-sm motion-delay-1400 hover:bg-base-300"
			>
				<figure
					class="flex flex-shrink-0 items-center justify-center rounded-md bg-gsupps-dark p-2"
				>
					<GSupps className="w-8 h-8 fill-white" />
				</figure>
				<div class="card-body min-w-0">
					<h2 class="pointer-events-none card-title">GSupps</h2>
					<div class="card-actions justify-end"></div>
				</div>
			</a>

			<!-- Throne -->

			<a
				href="https://throne.com/sukii"
				class="card card-side w-full motion-preset-slide-right bg-black shadow-sm motion-delay-1600 hover:bg-base-300"
			>
				<figure
					class="flex flex-shrink-0 items-center justify-center rounded-md bg-throne-blue p-2"
				>
					<Throne className="w-8 h-8 fill-white" />
				</figure>
				<div class="card-body min-w-0">
					<h2 class="pointer-events-none card-title">Throne</h2>
					<div class="card-actions justify-end"></div>
				</div>
			</a>
		</div>
	</div>
</div>

<style>
	.clip-diagonal {
		clip-path: polygon(0 0, 100% 0, 100% calc(100% - 80px), 0 100%);
	}
</style>
