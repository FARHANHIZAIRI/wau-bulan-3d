# Wau GLB dan kod embed

Empat fail GLB berada dalam `wau/assets/`: `jala.glb`, `kucing.glb`, `seri.glb`, `bulan.glb`.
Setiap fail mengandungi tekstur terbenam, empat mesh (Kepala, Sayap kiri, Sayap kanan, Ekor), dan dua klip animasi `Pisahkan` dan `Cantumkan` (1.4 saat setiap satu). Tetapkan klip kepada play once / clamp di penghujung untuk mengekalkan kedudukan. Model asal tidak diubah.

## Embed dengan popup maklumat

1. Upload seluruh folder `wau` ke root awam laman web, supaya URL `/wau/index.html` boleh dibuka.
2. Tampal kod daripada `embed-code.html.txt` ke blok Custom HTML / Embed pada laman you.
3. Tukar `model=kucing` kepada `model=jala`, `model=seri` atau `model=bulan` untuk memilih model awal.
4. Jika folder berada di lokasi lain, ubah `src` iframe kepada URL sebenar. Paparan boleh memerlukan ketinggian iframe lebih besar pada telefon; nilai `height` boleh diubah.

Popup maklumat disediakan oleh kod web. GLB menyimpan mesh, tekstur, animasi dan metadata penerangan; popup HTML tidak dapat disimpan sebagai UI interaktif di dalam format GLB. Corak ialah tekstur permukaan dan diperlihatkan melalui paparan dekat. GLB mempunyai potongan terbuka pada sambungan hasil pemisahan mesh; bukan komponen CAD pembinaan.

Viewer dalam pakej menggunakan GLB ini secara terus, tanpa CDN Three.js. Fon mempunyai fon pengganti jika tiada Internet. Muatkan melalui HTTP/HTTPS, bukan `file://`. Pakej tidak mengandungi URL hosting yang sudah diterbitkan.
