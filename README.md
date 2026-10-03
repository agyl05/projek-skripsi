# projek-skripsi
"Klasifikasi Hama dan Penyakit Tanaman Daun Cabai Menggunakan ConvNeXt V2 Berbasis Masked Autoencoders"
# Deskripsi projek:
projek ini merupakan implementasi Deep Learning untuk melakukan klasifikasi citra daun cabai berdasarkan kondisi visual daun menggunakan arsitektur ConvNeXt V2 berbasis Masked Autoencoders (MAE). projek ini dibuat sebagai bagian dari penelitian skripsi dengan tujuan mengklasifikasikan citra daun cabai ke dalam beberapa kategori berdasarkan karakteristik visual yang terdapat pada citra.
# Kategori Klasifikasi:
Leaf Curl, Whitefly, Yellowish, Leaf Spot, Healthy.
## Dataset
- Sumber: Kaggle (https://www.kaggle.com/datasets/crewsat/chili-leaf-disease-image-dataset)(https://www.kaggle.com/datasets/alinedobrovsky/plant-disease-classification-merged-dataset)(https://www.kaggle.com/datasets/ratnasarii/penyakitdauncabai)(https://www.kaggle.com/datasets/aagusw90/dauncabai)
- Total: 2.100 gambar, 5 kelas
- Pembagian: 80:10:10 (train/validation/test), stratified
# metode yang digunakan:
1. Pengumpulan Dataset
2. Preprocessing citra
3. Pembagian dataset
4. Implementasi ConvNeXt V2 Tiny
5. Training dua fase
   - Fase 1 (feature extraction) : learnign rate 1e-3
   - Fase 2 (fine-tuning) : learning rate backbone 5e-6, head 1e-4
6. Evaluasi Model
7. Interpretasi prediksi dengan Grad-CAM
# Tools yang digunakan:
Python, PyTorch, timm, Google Colab, ConvNeXt V2, Masked Autoencoders (MAE)
# metrik evaluasi:
Accuracy, Precision, Recall, F1-Score, Confusion Matrix.
# hasil 
Model dilatih dengan augmentasi data dan dievaluasi pada 210 gambar uji
- Accuracy 95,71%
- Precision (macro) 95,71%
- Recall (macro) 95,71%
- F1-Score (macro) 95,71%
- ROC-AUC (macro) 0,9976

