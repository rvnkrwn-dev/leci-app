<template>
  <div class="w-full max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 py-12 md:py-20">
    <header>
      <h1 class="section-title">Syarat & Ketentuan</h1>
    </header>

    <main>
      <div class="cyber-card p-6 md:p-10 privacy-content">
        <p><strong>Tanggal Efektif:</strong> 4 September 2025</p>
        <p>Harap baca Syarat dan Ketentuan ini dengan saksama sebelum menggunakan layanan yang ditawarkan oleh Leci
          Digital Solutions. Dengan menggunakan layanan kami, Anda setuju untuk terikat oleh syarat dan ketentuan
          ini.</p>

        <h3>1. Definisi Layanan</h3>
        <p>Leci Digital Solutions menyediakan layanan pengembangan perangkat lunak, termasuk pembuatan website, aplikasi
          web, desain UI/UX, dan layanan terkait lainnya seperti yang dijelaskan dalam paket layanan kami atau proposal
          proyek kustom.</p>

        <h3>2. Lingkup Pekerjaan & Revisi</h3>
        <p>Lingkup pekerjaan akan ditentukan dalam proposal atau faktur awal. Setiap pekerjaan tambahan atau perubahan
          di luar lingkup yang disepakati akan dianggap sebagai pekerjaan baru dan mungkin dikenakan biaya tambahan.
          Jumlah revisi desain atau fungsionalitas terbatas sesuai dengan paket layanan yang dipilih.</p>

        <h3>3. Kewajiban Klien</h3>
        <p>Klien setuju untuk menyediakan semua materi yang diperlukan (teks, gambar, logo) secara tepat waktu.
          Keterlambatan dalam penyediaan materi dapat mempengaruhi jadwal penyelesaian proyek. Klien bertanggung jawab
          penuh atas keakuratan dan hak cipta dari semua materi yang diberikan.</p>

        <h3>4. Pembayaran</h3>
        <p>Jadwal pembayaran standar adalah uang muka sebesar 50% sebelum pekerjaan dimulai, dan pelunasan 50% setelah
          proyek selesai dan sebelum serah terima akhir (go-live). Jadwal pembayaran lain dapat disepakati dalam
          proposal proyek. Semua pembayaran tidak dapat dikembalikan.</p>

        <h3>5. Hak Kekayaan Intelektual</h3>
        <p>Setelah pembayaran penuh diterima, hak cipta atas desain akhir dan kode situs web akan menjadi milik klien.
          Kami berhak untuk menampilkan proyek yang telah selesai dalam portofolio kami dan materi promosi lainnya.</p>

        <h3>6. Batasan Tanggung Jawab</h3>
        <p>Leci Digital Solutions tidak akan bertanggung jawab atas kerugian tidak langsung, insidental, atau
          konsekuensial yang timbul dari penggunaan atau ketidakmampuan untuk menggunakan layanan kami. Tanggung jawab
          total kami atas klaim apa pun tidak akan melebihi jumlah total yang dibayarkan oleh klien untuk layanan
          tersebut.</p>

        <h3>7. Garansi</h3>
        <p>Kami memberikan garansi perbaikan bug atau kesalahan teknis yang berasal dari kode kami selama 30 hari
          setelah peluncuran situs. Garansi ini tidak mencakup masalah yang disebabkan oleh perubahan yang dilakukan
          oleh klien atau pihak ketiga, atau masalah yang berkaitan dengan hosting pihak ketiga.</p>

        <h3>8. Perubahan pada Syarat & Ketentuan</h3>
        <p>Kami berhak untuk mengubah syarat dan ketentuan ini dari waktu ke waktu. Versi terbaru akan selalu tersedia
          di situs web kami. Penggunaan layanan kami secara berkelanjutan setelah perubahan tersebut merupakan
          penerimaan Anda terhadap syarat dan ketentuan yang baru.</p>

        <h3>9. Hubungi Kami</h3>
        <p>Jika Anda memiliki pertanyaan tentang Syarat & Ketentuan ini, silakan hubungi kami di:</p>
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
  title: 'Syarat & Ketentuan - Leci Digital Solutions',
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
