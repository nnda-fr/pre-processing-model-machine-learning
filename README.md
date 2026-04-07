# California Housing: End-to-End Machine Learning Project Workflow
Repositori ini berisi implementasi lengkap alur kerja Machine Learning untuk dataset California Housing, mencakup teknik Unsupervised Learning (clustering) dan Supervised Learning (classification)

Ringkasan Proyek ini bertujuan untuk melakukan segmentasi wilayah perumahan dan memambangun model prediksi yang telah dioptimasi.

Alur Kerja Notebook
1. Tahap Clustering
   
   A. Data Preprocessing: 
   * Feature Selection: menghapus kolom yang tidak relevan (Date, ID, IP, Address).
   * Feature Encoding: menggunakan LabelEncoder untuk fitur kategorikal.
   * Outlier Handling: Pembersihan outlier menggunakan metode drop
   * Feature Scaling: standardisasi fitur numerik dengan StandardScaler.
     
   B. Modeling:
   * penentuan jumlah cluster optimal menggunakan Elbow Method dengan KEIbowVisualizer.
   * implementasi algoritma K-Means Clustering.
   * Evaluasi model menggunakan Silhouette Score.
   * Reduksi dimensi menggunakan PCA untuk perbandingan model.
     
   C. Post Clustering:
   * inverse transform: mengembalikan data ke rentang normal untuk analisis deskriptif hasil cluster.
     
3. Tahap Classification
   * menggunakan hasil clustering  sebagai label target.
   * pembagian data menjadi training dan testing set menggunakan metode 20/80.
   * membangun model dasar menggunakan Decision Tree.
   * melatih model kompetitor untuk perbandingan menggunakan random forest classifier.
   * melakukan hyperparameter tuning.
     

