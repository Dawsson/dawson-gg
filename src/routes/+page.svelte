<script lang="ts">
    import discord from "$lib/images/discord-mark-blue.svg"
    import github from "$lib/images/github-mark.svg"
</script>

<div class="container h-full mx-auto flex justify-center items-center text-2xl">
	<div class="space-y-36 text-center flex flex-col items-center">
		<div class="space-y-5">
			<h1 class="h1">Hey, I'm Dawson</h1>

			<div class="flex justify-center space-x-2">
				<p>
					I'm Dawson, a fullstack developer based in Michigan. My primary focus is creating products for <a class="hover:brightness-125 ease-in-out duration-100" href="https://flyte.gg"><strong>Flyte.</strong></a>
					<br>
					My coding experience consists of Kotlin, Java, Typescript, Lua, and Python with experience in other tools such as Cloudflare, Linux, and Domain Management.
				</p>
			</div>
		</div>

		<div class="space-y-5">
			<h1 class="h1">Contact Me</h1>

			<p>
				I am willing to talk about anything. Contact me with a DM for a quick response, or
				<br>
				for more serious enquiries reach me at <a class="hover:brightness-125 underline decoration-dotted ease-in-out duration-100" href="mailto:hello@dawson.gg">hello@dawson.gg.</a>
			</p>

            <div class="py-4">
				<a href="https://github.com/Dawsson" target="_blank" class="inline-flex items-center justify-center size-32 hover:scale-105 ease-in-out duration-150"><img src="{discord}" alt="Blue Discord Mark"></a>

				<a href="https://github.com/Dawsson" target="_blank" class="inline-flex items-center justify-center size-32 hover:scale-105 ease-in-out duration-150"><img src="{github}" alt="Github Mark"></a>
            </div>
		</div>
	</div>
</div>

<style lang="postcss">
	figure {
		@apply flex relative flex-col;
	}
	figure svg,
	.img-bg {
		@apply w-64 h-64 md:w-80 md:h-80;
	}
	.img-bg {
		@apply absolute z-[-1] rounded-full blur-[50px] transition-all;
		animation: pulse 5s cubic-bezier(0, 0, 0, 0.5) infinite,
			glow 5s linear infinite;
	}
	@keyframes glow {
		0% {
			@apply bg-primary-400/50;
		}
		33% {
			@apply bg-secondary-400/50;
		}
		66% {
			@apply bg-tertiary-400/50;
		}
		100% {
			@apply bg-primary-400/50;
		}
	}
	@keyframes pulse {
		50% {
			transform: scale(1.5);
		}
	}
</style>
