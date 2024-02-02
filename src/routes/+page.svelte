<script>
	import { fade } from 'svelte/transition';
	let stage = 0;
</script>

<div class="bg-black h-screen text-white flex flex-col justify-center items-center p-4 gap-4">
	{#if stage === 0}
		<h1 class="text-2xl font-bold">🎉Happy birthday🎉</h1>
		<h1 class="text-xl font-bold">BABYY!🥳</h1>
		<img class="mt-4 w-32 h-32 object-cover rounded-full" src="/baby1.png " alt="" />

		<button class="btn bg-blue-400 mt-4 rounded-md p-2 font-bold" on:click={() => stage++}
			>Pencet ini babe</button
		>
	{/if}
	{#if stage === 1}
		<div in:fade={{ duration: 300 }}>
			<h1 class="text-2xl font-bold">Bayi manja aku sekarang</h1>
			<h1 class="text-6xl font-bold">22 <span class="text-2xl">Tahun 🥰</span></h1>

			<button
				in:fade={{ duration: 500, delay: 1000 }}
				class="btn bg-blue-400 mt-4 rounded-md p-2 font-bold"
				on:click={() => stage++}>Pencet ini babe</button
			>
		</div>
	{/if}
	{#if stage === 2}
		<h1 in:fade={{ duration: 1500, delay: 500 }} class="text-2xl font-bold">
			Foto tercantik baby 21 ✨
		</h1>
		<div
			in:fade={{ duration: 1500, delay: 2000 }}
			class="flex justify-center items-center flex-wrap gap-4"
		>
			<img class="w-24" src="/baby3.jpg" alt="" />
			<img class="w-24" src="/baby4.jpg" alt="" />
			<img class="w-24" src="/baby5.jpg" alt="" />
			<img class="w-24" src="/baby6.jpg" alt="" />
			<img class="w-24" src="/baby2.jpg" alt="" />
			<img class="w-24" src="/baby7.jpg" alt="" />
		</div>
		<button
			in:fade={{ duration: 1500, delay: 3000 }}
			class="btn bg-blue-400 mt-4 rounded-md p-2 font-bold"
			on:click={() => stage++}>Pencet ini babe</button
		>
	{/if}
	{#if stage === 3}
		<h1 in:fade={{ duration: 1000, delay: 500 }} class="text-2xl font-bold">
			Masakan terenak baby 😋
		</h1>
		<div
			in:fade={{ duration: 1000, delay: 500 }}
			class="flex justify-center items-center flex-wrap gap-4"
		>
			<img class="w-32" src="/baby8.jpg" alt="" />
		</div>
		<button
			in:fade={{ duration: 1000, delay: 1000 }}
			class="btn bg-blue-400 mt-4 rounded-md p-2 font-bold"
			on:click={() => stage++}>Pencet ini babe</button
		>
	{/if}

	{#if stage === 4}
		<img
			in:fade={{ duration: 1000, delay: 500 }}
			on:click={() => stage++}
			src="/baby9.png"
			alt=""
		/>
		<h1 in:fade={{ duration: 1000, delay: 1000 }} class="font-bold text-xl mt-2">
			Buka kadonya baby!
		</h1>
	{/if}

	{#if stage === 5}
		<div class="flex" in:fade={{ duration: 1000, delay: 500 }}>
			<img class="w-32 h-32" src="/baby11.png" alt="" />
			<img class="w-36 h-32" src="/baby10.png" alt="" />
		</div>
		<h1 in:fade={{ duration: 1000, delay: 1000 }} class="font-bold text-xl mt-2 text-justify">
			I love you baby! Semoga setiap doa kamu dikabulkan, derajat kamu dinaikan, semua harapan dan
			usaha kamu tercapai.
		</h1>

		<h1 in:fade={{ duration: 1000, delay: 1500 }} class="font-bold text-xl mt-2 text-justify">
			Semoga di umur 22 tahun ini kamu tambah sholeh, ibadahnay tambah rajin, dan semakin sukses.
			Aamiin 🤲
		</h1>

		<h1 in:fade={{ duration: 1000, delay: 2000 }} class="font-bold text-xl mt-2 text-justify">
			اللَّهُمَّ إِنِّي أَسْأَلُكَ الْعَفْوَ وَالْعَافِيَةَ فِي الدُّنْيَا وَالْآخِرَةِ Artinya: "Ya
			Allah, aku memohon pengampunan dan keselamatan di dunia dan akhirat." (HR Tirmidzi & Ibnu
			Majah)
		</h1>

		<button
			in:fade={{ duration: 1000, delay: 2500 }}
			class="btn bg-blue-400 mt-4 rounded-md p-2 font-bold"
			on:click={() => stage++}>Pencet ini babe</button
		>
	{/if}

	{#if stage === 6}
		<h1 in:fade={{ duration: 1000, delay: 1000 }} class="text-2xl font-bold">I love you 💖</h1>
		<div
			in:fade={{ duration: 1000, delay: 2000 }}
			class="flex justify-center items-center flex-wrap gap-4"
		>
			<img class="w-40" src="/baby12.jpg" alt="" />
		</div>
	{/if}
</div>
