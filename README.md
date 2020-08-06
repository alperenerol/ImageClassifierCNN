# ImageClassifierCNN
AÇIKLAMA:

Model verilen dataset'teki 7 farklı meyve sınıfına göre train edildi, trainModelParams.pth dosyası train edilmiş modelin parametrelerini içerir, train.py trainingden sonra bu dosyayı kaydeder. inference.py bu dosyayı kullanarak tekrardan traininge gerek kalmadan modelin çalışmasını sağlar.

Kullanılacak Dataset'te dosya dizilimi dataset/class/xxx.jpg şeklinde olmalıdır, yani verilen dataset'teki gibi.

Kodun çalışması için tüm fotoğrafların aynı boyutta olması gerektiğinden prediction öncesinde datasetteki fotoğraflar min(width, height) 'a göre kare halini almakta daha sonra ise 100x100 luk boyutlara resize olmakta ve imajlar tempInference adındaki klasöre geçici olarak kaydolmaktadır, program bu klasörü dataset olacak şekilde yükler.


Nasıl Çalıştırılır?

-Prediction kodunun çalışması için kullanılacak datasetin path'i (inference.py)'de belirtilmeli. 

-Meyve türü/sınıfı sayısı num_classes kısmında belirtilmelidir. Şuanda 7 olarak ayarlandı. Daha farklı sayıda meyve sınıfı ile modeli kullanmak için yeniden train edilmelidir.

Bu kadar, sonrasında terminalde run edilebilir.
