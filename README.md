
# Image Classification - MobileNetV2 Transfer Learning

## Deskripsi Project
Project ini adalah implementasi klasifikasi gambar menggunakan **Transfer Learning MobileNetV2** dengan TensorFlow dan Keras untuk mengidentifikasi beberapa jenis bunga pada dataset Flower Photos.

Model dibangun menggunakan arsitektur Sequential dengan tambahan layer CNN eksplisit seperti Conv2D dan MaxPooling2D untuk memenuhi implementasi dasar Convolutional Neural Network (CNN), serta memanfaatkan pretrained weights ImageNet dari MobileNetV2 untuk meningkatkan performa klasifikasi dan generalisasi model.

---

## Dataset
- Dataset: Flower Photos Dataset
- Total kelas: 5 kelas bunga
- Jumlah dataset: >3000 gambar
- Dataset dibagi menjadi:
  - Training Set
  - Validation Set
  - Testing Set

---

## Arsitektur Model

Model menggunakan kombinasi CNN Sequential dan Transfer Learning dengan struktur:

- Sequential Model
- MobileNetV2 (Pretrained ImageNet, include_top=False)
- Conv2D Layer
- MaxPooling2D Layer
- GlobalAveragePooling2D
- BatchNormalization
- Dense Layer (256 neuron, ReLU)
- Dropout (0.5)
- Output Layer (Softmax)

---

## Teknik Training

### Transfer Learning
- Menggunakan MobileNetV2 pretrained ImageNet
- Base model dibekukan (frozen) saat training

### Data Augmentation
- Rotation
- Zoom
- Width Shift
- Height Shift
- Brightness Adjustment
- Horizontal Flip

### Optimizer dan Callback
- Optimizer: Adam
- Learning Rate: 0.0003
- Callback:
  - EarlyStopping
  - ReduceLROnPlateau

---

## Hasil Evaluasi Model

### Accuracy
- Training Accuracy: **98.40%**
- Validation Accuracy: **89.95%**
- Test Accuracy: **89.75%**

### Loss
- Test Loss: **0.3186**

---

## Analisis Performa

Model menunjukkan performa klasifikasi yang sangat baik dengan akurasi testing mendekati 90%.

Beberapa faktor yang membantu peningkatan performa model:
- Penggunaan pretrained MobileNetV2 sebagai feature extractor
- Data augmentation untuk meningkatkan generalisasi
- BatchNormalization dan Dropout untuk mengurangi overfitting
- Callback learning rate scheduler untuk stabilitas training

Perbedaan antara training accuracy dan validation accuracy menunjukkan model memiliki kemampuan pembelajaran yang sangat tinggi pada training set, namun masih mampu mempertahankan generalisasi yang baik pada validation dan testing set.

---

## Format Model Output

Model berhasil dikonversi ke beberapa format deployment:

- SavedModel
- TensorFlow Lite (TFLite)
- TensorFlow.js (TFJS)

---

## Kesimpulan

Project ini berhasil mengimplementasikan kombinasi CNN Sequential dan Transfer Learning MobileNetV2 untuk klasifikasi gambar bunga dengan performa tinggi.

Dengan tambahan Conv2D dan MaxPooling2D secara eksplisit, model tetap memenuhi kriteria implementasi CNN dasar sekaligus memperoleh keuntungan dari transfer learning modern.

Model mencapai:
- Akurasi training di atas 98%
- Akurasi validation dan testing mendekati 90%
- Generalisasi model yang stabil
- Dukungan deployment multi-platform melalui SavedModel, TFLite, dan TensorFlow.js
