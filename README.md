# smart-logistics-supply-chain-prediction-model

## About Project
Dalam dunia "supply & demand" proses logistik sering terjadi dan juga cukup menantang bagi para penyedia, kita tidak bisa pungkiri proses logistik merupakan peranan penting dalam memenuhi "demand" yang terus meningkat seiring berkembangnya teknologi. Proses logistik dalam membantu ketersediaan (supply) ini juga penting dalam perputaran ekonomi, pasalnya "supply & demand" tidak akan berjalan tanpa adanya proses logistik yang baik. Walaupun terkadang dalam proses logistik banyak faktor yang dapat menghambat sehingga proses logistik dapat tertunda dan perputaran ekonomi terganggu. Namun, saaat ini kita mampu untuk mengatasi hal tersebut dengan mengoptimasi melalui model machine learning untuk melakukan prediksi apakah proses logistik tertunda atau tidak yang akan ktia lakukan dalam proyek ini.

## Model
Dengan menggunakan Grid_search memudahkan kita akan lebih mudah memahami tuning dari model yang ingin digunakan. Dari hasil menggunakan Grid Search kita menemukan parameter dan akurasi terbaik, mulai dari regularisai (C) dengan nilai 1, dan pemanfaat 'l1' dan solver menggunkan 'liblinear' lebih cocok dalam menangani bias dan varians dengan lebih baik.

## Evaluation
Secara keseluruhan hasil dari model ini cukup baik dalam memprediksi true positive dan true negative begitu juga dengan false positive dan false negative. Peningkatan model masih memungkinkan untuk mendapatkan model yang lebih sensitif pada fitur tertentu. Tetapi harus mempertimbangkan kendala overfitting ataupun underfitting. Untuk meningkatkan sensitifias dari fitur tertentu bisa kita ketahui dari feature importance. Berdasarkan model ini feature importance (fitur yang paling mempengaruhi) ada pada fitur Traffic_Status. Jika kita ingin melakukan prediksi dengan acuan fitur yang berbeda kita bisa melakukan pengklasifikasian yang berbeda dengan fitur tertentu untuk dijadikan sebagai variabel target.

## Conclusion
Jadi dari hasil yang telah dilakukan menggunakan model logistic regression dengan parameter regularisai (C) dengan nilai 1, dan pemanfaat 'l1' dan solver menggunkan 'liblinear' lebih cocok dalam menangani bias dan varians. Model juga sudah baik dalam memprediksi Delay dan No Delay.

Sensitivitas model bisa disesuaikan jika ingin dipriotitaskan untuk meminmilisir false positive, melalui fitur yang ada contohnya seperti User_Purchase_Frequency, dan buat lebih klasifikasi yang spesifik pada status Logistics_Delay_Reason.
