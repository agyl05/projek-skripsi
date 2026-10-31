# proyek-skripsi
# Klasifikasi Penyakit dan Hama Daun Cabai Menggunakan ConvNeXt V2 Berbasis Masked Autoencoders
Klasifikasi 5 kondisi daun cabai dengan ConvNeXt V2 Tiny. **Akurasi uji 95,71%** pada 210 gambar uji (ROC-AUC 0,9976).
## Deskripsi Proyek
Proyek ini merupakan implementasi deep learning untuk mengklasifikasikan citra daun cabai berdasarkan kondisi visualnya, menggunakan arsitektur ConvNeXt V2 berbasis Masked Autoencoders (MAE). Proyek ini dibuat sebagai bagian dari penelitian skripsi, dengan tujuan mengelompokkan citra daun ke dalam lima kategori berdasarkan karakteristik visual pada citra.
## Kategori Klasifikasi:
Leaf Curl, Whitefly, Yellowish, Leaf Spot, Healthy.
## Dataset
- Sumber: Kaggle (https://www.kaggle.com/datasets/crewsat/chili-leaf-disease-image-dataset)(https://www.kaggle.com/datasets/alinedobrovsky/plant-disease-classification-merged-dataset)(https://www.kaggle.com/datasets/ratnasarii/penyakitdauncabai)(https://www.kaggle.com/datasets/aagusw90/dauncabai)
- Total: 2.100 gambar, 5 kelas
- Pembagian: 80:10:10 (train/validation/test), stratified
## metode yang digunakan:
1. Pengumpulan Dataset
2. Preprocessing citra
3. Pembagian dataset
4. Implementasi ConvNeXt V2 Tiny
5. Training dua fase
   - Fase 1 (feature extraction) : learnign rate 1e-3
   - Fase 2 (fine-tuning) : learning rate backbone 5e-6, head 1e-4
6. Evaluasi Model
7. Interpretasi prediksi dengan Grad-CAM
## Tools yang digunakan:
Python, PyTorch, timm, Google Colab, ConvNeXt V2, Masked Autoencoders (MAE)
## metrik evaluasi:
Accuracy, Precision, Recall, F1-Score, Confusion Matrix.
## hasil 
Model dilatih dengan augmentasi data dan dievaluasi pada 210 gambar uji
- Accuracy 95,71%
- Precision (macro) 95,71%
- Recall (macro) 95,71%
- F1-Score (macro) 95,71%
- ROC-AUC (macro) 0,9976

