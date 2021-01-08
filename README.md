# Peringkasan Teks Berita Bahasa Inggris dengan Strategi Ekstraktif menggunakan Algoritma Text Rank

## Dataset:
1. BBC News Summary (https://www.kaggle.com/pariza/bbc-news-summary)
2. Glove Data (http://nlp.stanford.edu/data/glove.6B.zip)

## Analisis Data
Word Frequency : Pada dataset dilakukan perhitungan frekuensi kata pada artikel dan ringkasannya asing - masing
Vocabulary Frequency : Pada dataset, dilakukan perhitungan frekuensi vocabulary yaitu jumlah kata yang unik per total kata dalam teks

## Preprocessing
Untuk mengimplementasikan algoritma TextRank untuk proyek ini, dataset harus diproses terlebih dahulu. Langkah-langkah yang dilakukan sampai menghasilkan vektor kalimat yaitu : 
1. Memisahkan beberapa paragraf menjadi kalimat terpisah yang disebut Sentence Segmentation, yaitu tahapan memecah paragraf atau teks menjadi kumpulan kalimat berdasarkan tanda pemisah kalimat. Pemisahan kalimat dapat dilakukan berdasarkan adanya simbol titik, simbol tanda tanya, atau simbol tanda seru
2. Menggunakan kata-kata stopwords dari nltk package dan menghapus karakter khusus, membersihkan kalimat (clean sentences) yang diekstrak dari langkah sebelumnya. Semua kalimat kemudian ditulis dengan huruf kecil (lower case).
 3. Kata-kata dari kalimat yang sudah dibersihkan kemudian diberi tokenized. Setiap kata dari kalimat tersebut diberi nilai token berdasarkan koefisien kata-kata yang disematkan (embedded wording coefficient).
4. Kata diubah menjadi representasi vektor (vector representation) menggunakan glove dan akhirnya kalimat menjadi representasi vektor dengan merata-ratakan semua vektor kata individual dalam sebuah kalimat.

## Implementasi
Pada proses implementasi, dimulai dari tahapan berikut.
1. Mengkompresi File
2. Preprocessing (Data Cleaning, Tokenization, Stopwords Removal)
3. Vector Representation of Sentences
4. Similarity Matrix Preparation
5. Implementasi Algoritma TextRank
