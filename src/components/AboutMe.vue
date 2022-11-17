<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					name: 'Kampus Merdeka',
					bio:
						'Kampus Merdeka adalah kebijakan yang dikeluarkan oleh Kemendikbudristek dengan memberikan hak kepada Mahasiswa untuk mengambil mata kuliah di luar program studi selama 1 semester dan berkegiatan di luar perguruan tinggi selama 2 semester. Perguruan tinggi diberikan kebebasan untuk menyediakan kegiatan Kampus Merdeka yang sesuai dengan kebutuhan dan minat mahasiswanya. Pengalaman Mahasiswa di kegiatan Kampus Merdeka akan berpengaruh besar terhadap kesiapan karir mahasiswa dengan cara memastikan Mahasiswa terus menyimak perubahan dunia luar kampus selama berkuliah dan dapat kesempatan untuk menerapkan ilmu kepada masalah di dunia nyata.',
				},
				{
					id: 2,
					name: `Program Studi Teknik Informatika Universitas Pasundan`,
					bio:
						'Teknik Informatika FT – Unpas, yang berdiri sejak tahun 1993 merupakan bagiandari keluarga Kampus Unpas. Selayaknya sebuah institusi pendidikan, tujuan utama prodi Teknik Informatika adalah menjadi wadah kita bersama menimba ilmu dan penddikan, yang bermanfaat bagi kehidupan diri, keluarga,  masyarakat, bangsa dan negara. Seperti kutipan Nelson Mandela: “Pendidikan adalah senjata paling mematikan, karena dengan itu Anda dapat mengubah dunia”. Pendidikan adalah sarana dan jalan kita untuk mengubah penghidupan dunia. Dengan berbekal kurikulum berbasis kompetensi, Prodi Teknik Informatika diharapkan menghasilkan lulusan yang kompeten di bidang rekayasa perangkat lunak, dengan riset kekhususan di bidang sistem informasi,  multimedia dan game, infrastruktur teknologi informasi, serta teknoprenership dan digital merkating. Terdapat kekhasan pembelajaran pemrograman yang diawali oleh metode berpikir komputasi, algoritma pemrograman, pemrograman web, mobile, serta internet of think. Besar harapan kami agar kami selalu dapat berkontribusi kepada masyarakat, khususnya di dunia Teknologi Informasi. Dengan membekali mahasiswa untuk selalu smart, endurance, and teamwork; diharapkan lulsan kami selain memilik hardskill, juga softskill serta tetap memiliki etika bermasyarakat.  Sesuai dengan karakter yang dikokohkan keluarga besar Paguyuban Psundan: pengkuh agamana, luhung elmuna, jembar budayana.',
				},
			],
		};
	},
};
</script>

<template>
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About profile image -->
		<div class="w-full sm:w-1/4 mb-7 sm:mb-0">
			<img
				src="../assets/images/logo-unpas.png"
				class="rounded-xl w-96"
				alt=""
			/>
		</div>

		<!-- About details -->
		<div class="w-full sm:w-3/4 text-left">
			<p
				v-for="bio in bios"
				:key="bio.id"
				class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg"
			>
			<b>{{bio.name}}</b> <br>
			
			{{ bio.bio }}
			</p>
		</div>
	</div>
</template>
