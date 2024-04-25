<script>
	import space from '$images/space.jpg?enhanced';
	import books from '$images/books.jpg?enhanced';
	import church from '$images/church.jpg?enhanced';

	import profile from '$images/profile.png?enhanced';
	import statue from '$images/statue.jpg?enhanced';
</script>

<svelte:head>
	<title>Adam Smith</title>
	<meta charset="UTF-8" />
	<meta name="description" content="Adam Smith" />
	<script type="application/ld+json">
    {
      "@context": "https://schema.org/",
      "@type": "Adam Smith",
      "name": "Adam Smith",
      "description": "Adam Smith"
    }
	</script>
	<meta name="keywords" content="Adam Smith, Adam, Smith" />
</svelte:head>

<div class="flex flex-col gap-16">
	<div class="flex rounded-xl overflow-hidden items-center max-lg:flex-col shadow">
		<enhanced:img
			priority={true}
			src={profile}
			class="min-w-[200px] h-auto z-10 scale-x-[-1] object-cover"
			alt="Danyel Koca"
		/>
		<div class="flex flex-col gap-8 p-8">
			<p class=" text-4xl">Adam Smith was an 18th-century Scottish philosopher.</p>
			<p class="font-bold text-md text-slate-500">
				He is considered the father of modern economics. Smith is most famous for his 1776 book, The
				Wealth of Nations. Smith's writings are studied by the most influential philosophers,
				writers, and economists.
			</p>
		</div>
	</div>
	<div>
		<p class=" text-3xl text-center mb-4">Wisdom from Smith</p>
		<div
			class="rounded-xl relative overflow-hidden shadow min-h-[100px] lg:min-h-[300px] flex items-center"
		>
			<enhanced:img
				src={statue}
				class="object-top filter grayscale opacity-30 h-full w-full object-cover absolute top-0 bottom-0 left-0 right-0 z-0"
				alt="Adam Smith Statue"
			/>
			<div class="flex flex-col gap-4 p-8">
				<p class="font-extrabold text-xl italic z-10">
					If justice is removed, the great, the immense fabric of human society, that fabric which
					to raise and support seems in this world [...] must in a moment crumble into atoms.
				</p>
				<p class="font-bold text-md text-slate-500 z-10">Adam Smith</p>
			</div>
		</div>
	</div>

	<div>
		<p class=" text-3xl text-center mb-4">Did you know?</p>
		<div class="grid grid-cols-3 gap-8">
			<div
				class="relative col-span-3 lg:col-span-1 flex w-full rounded-xl overflow-hidden min-h-[150px] lg:min-h-[300px]"
			>
				<enhanced:img
					src={space}
					class="h-full w-full object-cover absolute top-0 bottom-0 left-0 right-0 z-0"
					alt="There is an asteroid named after Adam Smith"
				/>
				<p
					class="font-bold text-lg z-10 text-slate-700 pb-4 flex h-full w-full items-end bg-gradient-to-b from-transparent to-slate-200 px-8"
				>
					There is an asteroid named after Smith.
				</p>
			</div>
			<div
				class="relative col-span-3 lg:col-span-1 flex w-full rounded-xl overflow-hidden min-h-[150px] lg:min-h-[300px]"
			>
				<enhanced:img
					src={church}
					class="h-full w-full object-cover absolute top-0 bottom-0 left-0 right-0 z-0"
					alt="Smith trained to be an Anglican priest, but never	took vows."
				/>
				<p
					class="font-bold text-lg z-10 text-slate-700 pb-4 flex h-full w-full items-end bg-gradient-to-b from-transparent to-slate-200 px-8"
				>
					Smith trained to be a priest, but never took vows.
				</p>
			</div>
			<div
				class="relative col-span-3 lg:col-span-1 flex w-full rounded-xl overflow-hidden min-h-[150px] lg:min-h-[300px]"
			>
				<enhanced:img
					src={books}
					class="h-full w-full object-cover absolute top-0 bottom-0 left-0 right-0 z-0"
					alt="Smith read all the time. His personal library consisted of nearly 1500 books."
				/>
				<p
					class="font-bold text-lg z-10 text-slate-700 pb-4 flex h-full w-full items-end bg-gradient-to-b from-transparent to-slate-200 px-8"
				>
					Smith read all the time. His personal library consisted of 1500 books.
				</p>
			</div>
		</div>
	</div>

	<div class="min-h-[200px] rounded-lg relative overflow-hidden flex justify-center items-center">
		<div class="rounded-bl-full h-full w-full absolute bg-pink-500/[0.5] z-0"></div>
		<div class="rounded-tr-full h-full w-full absolute bg-blue-500/[0.5] z-0"></div>
		<div class="rounded-br-full h-full w-full absolute bg-amber-500/[0.5] z-0"></div>
		<div class="rounded-tl-full h-full w-full absolute bg-fuchsia-500/[0.5] z-0"></div>
		<div class="flex gap-8 flex-col justify-center items-center">
			<p class="z-10 text-3xl text-center text-white">Want to learn more?</p>
			<button
				on:click={() => alert('Noted!')}
				class="z-10 rounded-full bg-blue-500 text-white px-8 py-2 font-bold">Get in touch!</button
			>
		</div>
	</div>
	<div class="flex flex-col gap-2">
		<div class="flex justify-center flex-row items-center">
			<span class="mr-1">This website scaffold was made by </span>
			<a target="_blank" class="text-blue-500 font-bold" href="https://danyelkoca.com/"
				>Danyel Koca</a
			>
			<span class="ml-1">in 2024 April.</span>
		</div>
		<div class="flex justify-center flex-row items-center">
			<span class="mr-1">Find the code </span>
			<a
				target="_blank"
				class="text-blue-500 font-bold"
				href="https://github.com/danyelkoca/scaffold">here</a
			>
			<span class="ml-1">on GitHub.</span>
		</div>
	</div>
</div>
