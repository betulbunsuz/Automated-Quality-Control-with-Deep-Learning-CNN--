🏭 Automated Quality Control with Deep Learning (CNN)
Bu proje, imalat sanayisinde kalite kontrol süreçlerini otomatize etmek amacıyla geliştirilmiştir. Manuel gözle kontrol süreçlerindeki insan hatasını minimize etmeyi hedefleyen bu sistem, CNN (Convolutional Neural Networks) kullanarak döküm ürünlerindeki (casting products) üretim hatalarını gerçek zamanlı olarak sınıflandırabilmektedir.

🛠️ Problem Statement
Geleneksel kalite kontrol süreçleri yavaş ve yorucudur. Bu projede:

Üretim bandından çıkan parçaların "Sağlam" (OK) veya "Kusurlu" (Defective) olarak anlık tespiti yapılmıştır.

Yapay zeka desteğiyle hata payı %X'in (Kendi başarın) altına indirilmiştir.

📊 Dataset & Preprocessing
Projede Kaggle - [Casting Product Image Data](https://www.kaggle.com/datasets/ravirajsinh45/real-life-industrial-dataset-of-casting-product/data) veri seti kullanılmıştır.

Veri seti, silindirik döküm parçalarının üstten çekilmiş fotoğraflarını içerir.

Data Augmentation: Modelin farklı ışık ve açı koşullarında da çalışabilmesi için görüntülere döndürme, zoom ve parlaklık gibi ön işlemler uygulanmıştır.

Normalization: Piksel değerleri 0-255 aralığından 0-1 aralığına çekilerek modelin daha hızlı yakınsaması (convergence) sağlanmıştır.

<img width="478" height="469" alt="image" src="https://github.com/user-attachments/assets/8fd8a6f1-1a5e-4638-8f7b-386d94810f5a" />

<img width="818" height="717" alt="image" src="https://github.com/user-attachments/assets/8d65bf91-2bb1-4b62-aef0-59fa04174a27" />




🧠 Model Architecture & Training
Model, derin öğrenme tabanlı bir Evrişimli Sinir Ağı (CNN) üzerine inşa edilmiştir:

Convolutional Layers: Görüntü üzerindeki kenar, doku ve kusur geometrilerini öğrenmek için.

Pooling Layers: Boyut küçültme ve en önemli özellikleri koruma amacıyla.

Dense Layers: Çıkarılan özelliklere dayanarak parçanın sınıfına (Ok/Def) karar vermek için.

📈 Performance Metrics
Modelin başarısı şu metriklerle doğrulanmıştır:

Accuracy: %... (Örn: 98.5)

Precision/Recall: Kusurlu ürünleri kaçırmama oranı (Recall) kritik olduğu için bu değerlere odaklanılmıştır.

Loss Curve: Eğitim ve doğrulama kaybı grafiklerinde aşırı öğrenme (overfitting) olmadığı gözlemlenmiştir.

<img width="1717" height="587" alt="image" src="https://github.com/user-attachments/assets/b4e894ae-f795-4daf-902e-87fe07b181ea" />


💻 Tech Stack
Frameworks: TensorFlow / Keras

Data Science: Pandas, NumPy

Computer Vision: OpenCV

Visualization: Matplotlib, Seaborn

📂 Project Structure
Plaintext
├── notebooks/          # Adım adım analiz ve modelleme 
└── README.md
🏁 Conclusion
Bu çalışma, Endüstri 4.0 kapsamında akıllı fabrikaların temel taşı olan "Sıfır Hata" (Zero Defect) prensibini desteklemektedir. Model, üretim hattına entegre edildiğinde maliyet tasarrufu ve verimlilik artışı sağlama potansiyeline sahiptir.
