<template>
  <div class="w-full max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 py-12 md:py-20">
    <header>
      <h1 class="section-title">Kebijakan Privasi</h1>
    </header>
    <main>
      <div class="cyber-card p-6 md:p-10 privacy-content">
        <p><strong>Tanggal Efektif:</strong> 4 September 2025</p>
        <p>Terima kasih telah mengunjungi situs web Leci Digital Solutions. Kami berkomitmen untuk melindungi privasi
          informasi pribadi Anda. Kebijakan Privasi ini menjelaskan bagaimana kami mengumpulkan, menggunakan,
          mengungkapkan, dan melindungi informasi Anda saat Anda mengunjungi situs web kami.</p>

        <h3>1. Informasi yang Kami Kumpulkan</h3>
        <p>Kami dapat mengumpulkan informasi pribadi yang Anda berikan secara sukarela kepada kami, seperti:</p>
        <ul>
          <li><strong>Informasi Kontak:</strong> Nama, alamat email, dan nomor telepon saat Anda mengisi formulir kontak
            kami.
          </li>
          <li><strong>Informasi Proyek:</strong> Detail mengenai kebutuhan proyek Anda yang Anda kirimkan melalui
            formulir permintaan atau konsultasi.
          </li>
        </ul>
        <p>Kami juga dapat mengumpulkan informasi non-pribadi secara otomatis saat Anda menavigasi situs, seperti alamat
          IP, jenis browser, sistem operasi, dan data penggunaan lainnya melalui cookie dan teknologi serupa.</p>

        <h3>2. Bagaimana Kami Menggunakan Informasi Anda</h3>
        <p>Kami menggunakan informasi yang kami kumpulkan untuk berbagai tujuan bisnis, termasuk:</p>
        <ul>
          <li>Untuk menanggapi pertanyaan Anda dan menyediakan layanan pelanggan.</li>
          <li>Untuk mengirimkan estimasi, proposal, dan informasi lain terkait layanan kami.</li>
          <li>Untuk meningkatkan dan mempersonalisasi pengalaman Anda di situs web kami.</li>
          <li>Untuk memantau dan menganalisis tren penggunaan dan aktivitas untuk tujuan pemasaran dan periklanan.</li>
        </ul>

        <h3>3. Berbagi Informasi Anda</h3>
        <p>Kami tidak menjual, memperdagangkan, atau menyewakan informasi identifikasi pribadi pengguna kepada pihak
          lain. Kami dapat membagikan informasi demografis gabungan yang tidak terkait dengan informasi pribadi apa pun
          mengenai pengunjung dan pengguna dengan mitra bisnis kami, afiliasi tepercaya, dan pengiklan untuk tujuan yang
          diuraikan di atas.</p>

        <h3>4. Keamanan Data</h3>
        <p>Kami mengadopsi praktik pengumpulan, penyimpanan, dan pemrosesan data yang sesuai serta langkah-langkah
          keamanan untuk melindungi dari akses, perubahan, pengungkapan, atau perusakan informasi pribadi Anda yang
          tidak sah.</p>

        <h3>5. Cookie dan Teknologi Pelacakan</h3>
        <p>Situs kami dapat menggunakan "cookie" untuk meningkatkan pengalaman pengguna. Browser web pengguna
          menempatkan cookie di hard drive mereka untuk tujuan pencatatan dan terkadang untuk melacak informasi tentang
          mereka. Anda dapat memilih untuk mengatur browser web Anda untuk menolak cookie, atau untuk memberi tahu Anda
          saat cookie dikirim.</p>

        <h3>6. Perubahan pada Kebijakan Privasi Ini</h3>
        <p>Leci Digital Solutions memiliki keleluasaan untuk memperbarui kebijakan privasi ini kapan saja. Ketika kami
          melakukannya, kami akan merevisi tanggal yang diperbarui di bagian atas halaman ini. Kami mendorong Pengguna
          untuk sering memeriksa halaman ini untuk setiap perubahan agar tetap mendapat informasi tentang bagaimana kami
          membantu melindungi informasi pribadi yang kami kumpulkan.</p>

        <h3>7. Hubungi Kami</h3>
        <p>Jika Anda memiliki pertanyaan tentang Kebijakan Privasi ini, praktik situs ini, atau urusan Anda dengan situs
          ini, silakan hubungi kami di:</p>
        <p><a href="mailto:halo@leci.app">halo@leci.app</a></p>
      </div>
    </main>
  </div>
</template>

<script setup>
definePageMeta({
  layout: false
})

// SEO and Meta Tags
useHead({
  title: 'Kebijakan Privasi - Leci Digital Solutions',
  htmlAttrs: {
    lang: 'id',
    class: 'scroll-smooth'
  },
  meta: [
    {name: 'robots', content: 'noindex, nofollow'}
  ],
});
</script>

<style>
.cyber-card {
  background-color: rgba(10, 10, 25, 0.6);
  border: 1px solid #2a9df4;
  box-shadow: 0 0 15px rgba(42, 157, 244, 0.4), inset 0 0 10px rgba(42, 157, 244, 0.2);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
}

.section-title {
  font-family: 'Orbitron', sans-serif;
  font-weight: 700;
  font-size: 2.25rem;
  text-align: center;
  margin-bottom: 2.5rem;
  color: #f0f0f0;
  text-shadow: 0 0 8px rgba(42, 157, 244, 0.7);
}

.privacy-content h3 {
  font-family: 'Orbitron', sans-serif;
  color: #2a9df4;
  font-size: 1.25rem;
  margin-top: 1.5rem;
  margin-bottom: 0.5rem;
}

.privacy-content p, .privacy-content ul {
  color: #d1d5db;
  margin-bottom: 1rem;
  line-height: 1.75;
}

.privacy-content ul {
  list-style-type: disc;
  padding-left: 1.5rem;
}

.privacy-content a {
  color: #67e8f9;
  text-decoration: underline;
  transition: color 0.3s ease;
}

.privacy-content a:hover {
  color: #f0abfc;
}
</style>
