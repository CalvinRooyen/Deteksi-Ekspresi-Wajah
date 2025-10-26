# Deteksi-Ekspresi-Wajah
🧠 Perbandingan Model VGG-16 dan ResNet-50 Menggunakan CNN pada Deteksi Ekspresi Wajah

Proyek ini membandingkan dua arsitektur Convolutional Neural Network (CNN) populer — VGG-16 dan ResNet-50 — dalam mendeteksi dua ekspresi wajah utama: senang dan takut, menggunakan dataset FER-2013.
Penelitian ini merupakan bagian dari tugas akhir oleh Calvin Rooyen Marcellino Christy (NIM: 215314143), Program Studi Informatika, Universitas Sanata Dharma.

📘 Deskripsi Proyek

Proyek ini bertujuan untuk:

Membandingkan performa VGG-16 dan ResNet-50 dalam mengenali ekspresi wajah.

Menganalisis pengaruh optimizer (Adam vs SGD) terhadap hasil pelatihan.

Mengevaluasi model berdasarkan accuracy, loss, confusion matrix, dan ROC-AUC Curve.

⚙️ Teknologi yang Digunakan

Python 3.10+

PyTorch

CUDA + cuDNN (untuk akselerasi GPU)

Google Colab / Jupyter Notebook

Matplotlib, NumPy, Torchvision, scikit-learn

🧪 Hasil Eksperimen
Model	Optimizer	Accuracy	Loss	AUC	Catatan
VGG-16	Adam	90.2%	0.22	0.94	Akurasi tinggi, stabil
ResNet-50	Adam	92.5%	0.18	0.96	Performa terbaik
VGG-16	SGD	87.8%	0.27	0.90	Konvergensi lambat
ResNet-50	SGD	89.7%	0.24	0.92	Stabil tapi kurang optimal
📊 Kesimpulan

ResNet-50 + Adam menghasilkan performa terbaik dengan accuracy 92.5% dan AUC 0.96.

VGG-16 + Adam tetap kompetitif dengan accuracy 90.2%.

Optimizer Adam memberikan hasil lebih baik daripada SGD dalam hal konvergensi dan stabilitas.

Model VGG-16 cocok untuk kasus ringan dengan data terbatas, sedangkan ResNet-50 unggul untuk presisi tinggi.
