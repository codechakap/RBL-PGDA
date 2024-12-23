# Abstract

RBL ini mengeksplorasi kelayakan penggunaan akuisisi data berbasis kereta untuk deteksi hujan secara real-time melalui Convolutional Neural Networks (CNN). Dengan memanfaatkan jaringan rel kereta yang luas sebagai platform sensor terdistribusi, Analisis ini menyelidiki potensi integrasi kamera onboard dengan algoritma CNN untuk menganalisis petunjuk visual terkait presipitasi. RBL ini menyajikan kerangka awal untuk sistem tersebut, mencakup strategi pengumpulan data, teknik pra-pemrosesan untuk data citra, serta arsitektur model CNN yang sesuai. Meskipun mengakui keterbatasan ketersediaan data untuk konsep awal ini, studi ini mengeksplorasi tantangan praktis dan potensi manfaat dari pendekatan inovatif ini, membuka jalan bagi penelitian dan pengembangan di masa depan dalam memanfaatkan infrastruktur yang ada untuk peningkatan pemantauan cuaca dan prakiraan. Model Convolutional Neural Network (CNN) dikembangkan dengan dataset _pratik2901/multiclass-weather-dataset_, model dapat mendeteksi hujan melalui gambar kamera dengan tingkat akurasi sebesar 98%. Hal ini menunjukkan bahwa model memiliki performa baik, mampu mempelajari pola-pola visual yang relevan secara efektif, seperti tetesan air, kabut, atau perubahan pencahayaan, yang merupakan indikator utama hujan dalam gambar kamera.

_Kata kunci: Akusisi data berbasis kereta, Computer Vision, Convolutional Neural Networks (CNNs), Pemantauan cuaca_

# Latar belakang

Curah hujan merupakan salah satu parameter utama dalam pemantauan kondisi cuaca dan iklim, yang memberikan dampak signifikan pada berbagai sektor, termasuk pertanian, pengelolaan sumber daya air, perencanaan perkotaan, dan mitigasi bencana. Pemantauan curah hujan yang akurat sangat diperlukan untuk mendukung pengambilan keputusan, terutama dalam pengelolaan risiko banjir dan kekeringan.

## Kekurangan Teknologi Konvensional

Teknologi konvensional, seperti stasiun cuaca dan pengukuran manual, sering kali memiliki keterbatasan dalam hal cakupan wilayah serta resolusi temporal. Di sisi lain, kamera yang telah banyak tersedia dapat dimanfaatkan untuk mendeteksi hujan secara langsung melalui citra visual.

## Solusi kami

Kemajuan teknologi kecerdasan buatan, khususnya Convolutional Neural Networks (CNN), membuka peluang baru untuk mendeteksi dan memprediksi curah hujan melalui analisis citra cuaca. CNN, yang dikenal unggul dalam pengolahan data visual, memungkinkan ekstraksi pola dan fitur penting dari data gambar yang diambil oleh kamera untuk mendeteksi curah hujan secara efektif.

# Metodologi

Pengumpulan data pada penelitian ini dilakukan menggunakan kereta api sebagai platform pengambilan citra visual. Kamera dipasang pada lokasi strategis di kereta untuk merekam citra visual sepanjang perjalanan dari satu stasiun ke stasiun berikutnya. Sebelum kereta meninggalkan stasiun awal, sistem pengambilan data diaktifkan untuk merekam citra sepanjang lintasan. Setelah tiba di stasiun tujuan, data citra yang telah terkumpul diunggah ke sistem penyimpanan lokal di stasiun tersebut. Selanjutnya, data tersebut ditransfer ke infrastruktur cloud untuk keperluan pemrosesan lebih lanjut.

Data yang telah diunggah ke cloud akan digunakan dalam pengembangan dan pengujian model CNN. Model ini dilatih untuk mengenali pola visual yang relevan dengan kondisi hujan berdasarkan citra yang diperoleh. Proses ini melibatkan tahap pra-pemrosesan data, pelabelan, dan validasi guna memastikan akurasi model dalam mendeteksi kondisi hujan. Dengan metode ini, pengumpulan dan pengolahan data dilakukan secara sistematis menggunakan kerangka kerja berbasis kereta api untuk mendukung pengembangan teknologi deteksi hujan berbasis visual.

# Kesimpulan

Model Convolutional Neural Network (CNN) yang dikembangkan untuk mendeteksi hujan melalui gambar kamera menunjukkan performa yang sangat baik, dengan tingkat akurasi sebesar 98% pada data validasi dan training. Hal ini menunjukkan bahwa model mampu mempelajari pola-pola visual yang relevan secara efektif, seperti tetesan air, kabut, atau perubahan pencahayaan, yang merupakan indikator utama hujan dalam gambar kamera.

Sebagai bagian dari proses pengembangan, data augmentation telah dilakukan untuk mengatasi keterbatasan jumlah data pelatihan. Teknik ini mencakup rotasi, flipping, translation, dan zooming pada gambar untuk menciptakan variasi data, sehingga membantu model mengenali pola-pola visual dari berbagai kondisi lingkungan. Hal ini turut berkontribusi pada kemampuan model untuk mencapai tingkat akurasi yang tinggi meskipun data pelatihan yang digunakan terbatas.

Namun, perlu diingat bahwa akurasi tinggi pada validasi dan pelatihan tidak selalu menjamin performa sempurna dalam kondisi nyata. Oleh karena itu, pengujian lebih lanjut dengan data dunia nyata yang lebih beragam, seperti perubahan pencahayaan ekstrem, kondisi kabur, atau kamera dengan resolusi rendah, perlu dilakukan untuk memastikan keandalan model dalam situasi yang lebih kompleks.

Dalam Research Based Learning(RBL) ini, kereta api akan dimanfaatkan sebagai medium atau sarana untuk pengambilan data terkait deteksi kondisi hujan. Penggunaan kereta api menawarkan keunggulan berupa cakupan wilayah yang luas dan lintasan yang terstandarisasi, sehingga memungkinkan pengumpulan data yang konsisten dan representatif. Kamera akan dipasang pada kereta api untuk merekam citra visual sepanjang perjalanan, yang kemudian digunakan sebagai data pelatihan bagi model CNN untuk mendeteksi hujan berdasarkan pola-pola visual yang teridentifikasi.

Tujuan dari pengembangan model CNN untuk deteksi hujan adalah menyediakan solusi teknologi yang efisien, akurat, dan dapat diandalkan dalam memantau curah hujan secara real-time. Dengan integrasi kereta api sebagai medium pengumpulan data, diharapkan model ini mampu menghasilkan data yang lebih beragam dan relevan untuk mendukung sistem pemantauan cuaca modern.

# Referensi

1. K. O’Shea and R. Nash, “An Introduction to Convolutional Neural Networks,”
   arXiv:1511.08458 [cs], vol. 2, Dec. 2015, Available: https://arxiv.org/abs/1511.08458

2. S. Russell and P. Norvig, “Artificial Intelligence A Modern Approach Third Edition,” 2010. Available: https://people.engr.tamu.edu/guni/csce421/files/AI_Russell_Norvig.pdf

3. M. Peter, D. Aldo, F. Cheng, and S. Ong, “MATHEMATICS FOR MACHINE LEARNING,” 2020. Available: https://mml-book.github.io/book/mml-book.pdf

4. F. Karabiber, “Binary Classification,” www.learndatasci.com. https://www.learndatasci.com/glossary/binary-classification/

5. J. Brownlee, “A Gentle Introduction to the Rectified Linear Unit (ReLU) for Deep Learning Neural Networks,” Machine Learning Mastery, Apr. 20, 2019. https://machinelearningmastery.com/rectified-linear-activation-function-for-deep-learning-neural-networks/

6. D. Liu, “A Practical Guide to ReLU,” Medium, Nov. 30, 2017. Available: https://medium.com/@danqing/a-practical-guide-to-relu-b83ca804f1f7

7. “Module: tf.keras | TensorFlow Core v2.4.1,” TensorFlow. https://www.tensorflow.org/api_docs/python/tf/keras

8. J. S. Cramer, “The Origins of Logistic Regression,” Nov. 2002. Available: https://papers.tinbergen.nl/02119.pdf

9. D. P. Kingma and J. Ba, “Adam: A Method for Stochastic Optimization,” arXiv.org, Dec. 22, 2014. https://arxiv.org/abs/1412.6980

10. V. Yathish, “Loss Functions and Their Use In Neural Networks,” Medium, Aug. 04, 2022. https://towardsdatascience.com/loss-functions-and-their-use-in-neural-networks-a470e703f1e9

11. Shiksha Online, “Cross Entropy Loss Function in Machine Learning - Shiksha Online,” Shiksha.com, Mar. 31, 2023. https://www.shiksha.com/online-courses/articles/cross-entropy-loss-function (accessed Dec. 22, 2024).

12. Pravin, “Guide For Loss Function in Tensorflow,” Analytics Vidhya, May 31, 2021. https://www.analyticsvidhya.com/blog/2021/05/guide-for-loss-function-in-tensorflow/ (accessed Dec. 22, 2024).

# Lembar Kontribusi

| No  | Name                       |    ID    | GitHub username                             | In charge activity                                              | Info with link                                                               | Shared max point |
| :-: | :------------------------- | :------: | :------------------------------------------ | :-------------------------------------------------------------- | :--------------------------------------------------------------------------- | :--------------: |
|  1  | Ahmad Royyan Fatah         | 10222065 | [ARoyyanF](https://github.com/ARoyyanF)     | Notebook: Machine learning, Notebook: Finalization, github repo | PLACEHOLDERnotebook, [Repository](https://github.com/ARoyyanF/RBL-PGDA/)     |        25        |
|  2  | Duke Ariqoh                | 10222016 | [dukeariqoh](https://github.com/dukeariqoh) | Slide on OSF, YouTube presenation video                         | [YouTube presenation video]([https://github.com/dukeariqoh](https://www.youtube.com/watch?v=8xEpNRD8BtQ))                                                                  |        25        |
|  3  | Nashwan Chakap Nanggala    | 10222036 | [codechakap](https://github.com/codechakap) | Notebook: Bandung dataset, Discussion on github Issues          | PLACEHOLDERnotebook, [issues](https://github.com/ARoyyanF/RBL-PGDA/issues/1) |        25        |
|  4  | Muhammad Fathin Abdul Aziz | 10222044 | [mfthn](https://github.com/mfthn)           | Notebook: Train simulation                                      | PLACEHOLDERnotebook                                                          |        25        |
