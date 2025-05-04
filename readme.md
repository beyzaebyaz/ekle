# NLP Ödevi – Mobil Uygulama Yorum Analizi

Bu proje, Google Play mağazasındaki Spotify kullanıcı yorumları üzerinden olumsuz geri bildirimleri analiz ederek en çok şikayet edilen başlıkları tespit etmeyi amaçlamaktadır. Çalışma, doğal dil işleme teknikleri ve Word2Vec / TF-IDF modelleme yöntemleri kullanılarak gerçekleştirilmiştir.

---

## 🔍 Proje Amacı

Mobil uygulama mağazalarında yapılan kullanıcı yorumları genellikle büyük miktarda veri içerir ve manuel olarak analiz edilmesi zordur. Bu projede, kullanıcıların en çok hangi konularda şikayet ettiğini anlamak için şu adımlar uygulanmıştır:

1. **Olumsuz yorumların filtrelenmesi**
2. **Verilerin ön işlenmesi (tokenization, stopword removal, lowercasing, lemmatization, stemming)**
3. **TF-IDF ve Word2Vec modelleme yöntemleriyle metinlerin sayısal gösterimi**
4. **Word2Vec ile semantik kümelerin analizi**
5. **Zipf yasasına göre kelime sıklığı dağılımı**
6. **En çok tekrar eden şikayet başlıklarının çıkarılması**

---

## 📂 Dosya Yapısı

```bash
📦project-root/
 ┣ 📂models/                  # Eğitilen 16 Word2Vec modeli
 ┣ 📂vectors/                 # TF-IDF çıktıları
 ┣ 📜task-1.ipynb             # Ön işleme ve analiz adımları
 ┣ 📜generate_tfidf_vectors.ipynb
 ┣ 📜train_word2vec_models.ipynb
 ┣ 📜zipf.ipynb               # Zipf grafikleri
 ┣ 📜README.md                # Bu dosya
 ┣ 📄reviews_cleaned_ultimate.csv
 ┣ 📄reviews_lemmatized.csv
 ┣ 📄reviews_stemmed.csv
