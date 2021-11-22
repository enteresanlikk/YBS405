# Ödev 1

https://raw.githubusercontent.com/yasarkucukefe/YBS_405/main/data/odev2veri.csv adresinden okuyacağınız veri setini kullanarak aşağıdaki sınıflandırma (classification) işlemlerini yapınız.

- Veri setindeki değişkenleri "standardize" ediniz. (ipucu: StandardScaler().fit_transform())
- Veri setindeki "TARGET CLASS" kolonu y, diğer kolonları X data frame'leri olarak ayırınız.
- Veri setinin %70'ini eğitim (training), %30'unu test verisi olarak ayırınız. (ipucu: train_test_split ile bir veri setini eğitim ve test olarak ayırabilirsiniz. https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html)
- Komşu sayısı 4 olan bir KNN sınıflandırma modeli oluşturunuz ve modelin doğruluk oranını hesaplayınız. (ipucu: KNeighborsClassifier())
- GridSearchCV kullarak model için en uygun komşu sayısını hesaplayınız. (n_neighbors parametresinin 2 ve 40 arasındaki değerleri için)
- Bulduğunuz en uygun komşu sayısı için modelin sağladığı doğruluk oranını eğitim ve test veri setleri için ayrı ayrı hesaplayınız.

- Bulduğunuz en uygun komşu sayısı için modelin performansını değerlendirmek amacıyla hata metrisini (confusion matrix) eğitim ve test veri setlerini kullanarak ayrı ayrı hesaplayınız.