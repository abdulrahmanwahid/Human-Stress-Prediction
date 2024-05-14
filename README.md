# Submission 1: Machine Learning Pipeline - Human Stress Prediction
Nama: Abdul Rahman Wahid

Username dicoding: abdulrahmanwahid

![human resources problems]([[https://user-images.githubusercontent.com/58927608/232183728-df31ce54-b58c-4163-a563-5df9d3daf167.jpg](https://www.istockphoto.com/id/foto-foto/stress](https://www.freepik.com/free-photo/portrait-asian-girl-feeling-headache-migraine-being-ill-standing-white-tshirt-white-background_23648342.htm#query=stress&position=9&from_view=keyword&track=sph&uuid=624f0291-a67d-4859-a539-c4a803a074bb)](https://images.theconversation.com/files/181154/original/file-20170807-16724-9vx8d1.jpg?ixlib=rb-4.1.0&q=45&auto=format&w=754&h=503&fit=crop&dpr=1))

[Sumber Gambar]([https://www.istockphoto.com/id/foto-foto/stress](https://www.freepik.com/free-photo/portrait-asian-girl-feeling-headache-migraine-being-ill-standing-white-tshirt-white-background_23648342.htm#query=stress&position=9&from_view=keyword&track=sph&uuid=624f0291-a67d-4859-a539-c4a803a074bb)](https://images.theconversation.com/files/181154/original/file-20170807-16724-9vx8d1.jpg?ixlib=rb-4.1.0&q=45&auto=format&w=754&h=503&fit=crop&dpr=1))

| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Human Stress Prediction](https://www.kaggle.com/datasets/kreeshrajani/human-stress-prediction) |
| Masalah | Stres adalah reaksi seseorang baik secara fisik maupun emosional (mental/psikis) apabila ada perubahan dari lingkungan yang mengharuskan seseorang menyesuaikan diri. Stres adalah bagian alami dan penting dari kehidupan, tetapi apabila berat dan berlangsung lama dapat merusak kesehatan |
| Solusi machine learning | Stress susah dilihat dari keseharian seseorang, oleh karena itu dengan machine learning dapat mengetahui apakah seseorang stress hanya dari ketikan seseorang yang dilakukan dimedia sosial |
| Metode pengolahan | Pada data Human Stress Prediction, terdapat tujuh feature, tetapi yang digunakan pada proyek ini hanya feature text dan label, sehingga features selain itu akan dihapus, kemudian dilakukan split data training dan eval menjadi rasio 80:20, dan mengubah data feature menjadi lowercase serta feature label menjadi integer |
| Arsitektur model | Arsitektur model yang digunakan yaitu model embedding dimana terdiri dari vectorize_layer, kemudian layer embedding dengan dimensi embedding yaitu 16, setelah itu layer AveragePooling1D karena data merupakan bentuk text, kemudian layer dense 64, 32 dengan activation relu dan sigmoid karena akan dilakukan klasifikasi antar dua label. Loss yang digunakan binary_crossentropy dengan optimizer Adam dan metrik BinaryAccuray |
| Metrik evaluasi | Metrik evaluasi yang digunakan yaitu ExampleCount, AUC, FalsePositives, TruePositives, FalseNegatives, TrueNegatives, dan BinaryAccuracy |
| Performa model | Evaluasi model diperoleh yaitu AUC sebesar 82%, kemudian example_count 575, dengan BinaryAccuracy 75%, dan loss sebesar 1.364. Untuk False Negatives 68, False Positive 75, True Negative 201 dan True Positive 231. Model yang telah dibuat dapat dilakukan peningkatan performa, karena model belum cukup baik karena BinaryAccuracy masih dibawah 80% |
