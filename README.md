# Image Classification - MobileNetV2 Transfer Learning

## Deskripsi Project
Project ini adalah model klasifikasi gambar menggunakan **Transfer Learning MobileNetV2** dengan TensorFlow dan Keras. Model dilatih untuk mengklasifikasikan gambar bunga ke dalam beberapa kelas menggunakan dataset Flower Photos.

Model ini dirancang untuk meningkatkan akurasi dan generalisasi dibandingkan CNN konvensional dengan memanfaatkan pretrained weights dari ImageNet.

---

## Dataset
- Flower Photos Dataset
- Total kelas: 5 kelas
- Dataset telah dibagi menjadi:
  - Training set
  - Validation set
  - Testing set

---

## Arsitektur Model
Model menggunakan pendekatan transfer learning dengan struktur:

- MobileNetV2 (Pretrained ImageNet, tanpa top layer)
- GlobalAveragePooling2D
- BatchNormalization
- Dense (256 neuron, ReLU)
- Dropout (0.5)
- Output layer (Softmax)

---

## Teknik Training
- Transfer Learning (Frozen base model)
- Data Augmentation:
  - Rotation
  - Zoom
  - Width/Height Shift
  - Brightness adjustment
  - Horizontal flip
- Optimizer: Adam (learning rate 0.0003)
- Callback:
  - EarlyStopping
  - ReduceLROnPlateau

---

## Hasil Evaluasi Model

- Training Accuracy: **0.8979 (89.79%)**
- Validation Accuracy: **0.8940 (89.40%)**
- Test Accuracy: **0.8921 (89.21%)**
- Test Loss: **0.3174**

---

## Analisis Performa
Model menunjukkan performa yang stabil dengan:
- Gap kecil antara training dan validation accuracy → tidak overfitting signifikan
- Loss rendah pada test set → generalisasi baik
- Akurasi mendekati 90% → memenuhi target evaluasi

---

## Format Model Output
Model disimpan dalam beberapa format untuk deployment:

- SavedModel (TensorFlow standard format)
- TensorFlow Lite (Mobile deployment)
- TensorFlow.js (Browser deployment)

---

## Kesimpulan
Model MobileNetV2 memberikan peningkatan signifikan dibandingkan CNN konvensional, dengan hasil yang lebih stabil, akurasi lebih tinggi, dan kemampuan generalisasi yang lebih baik pada dataset flower classification.