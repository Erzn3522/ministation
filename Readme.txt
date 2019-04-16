Biz bu projeyi yaparken karþýlaþtýðýmýz tek sorun kütüphaneler
ve fonksyonlarýn uyumsuzluðu oldu.Basýnç ölçümü için Bmp180 
sensörünü kullandýk.Bu sensör için ise 2 farklý kütüphane kullandýk

Ýlk baþta <Adafruit_BMP085.h> kütüphanesini kullandýðýmýzda bu fonksyonlar
kütüphanenin test kodlarýnda tanýmlý ve çalýþýyor olmasýna raðmen bu 
fonksyonlar bu kütüphanede tanýmlý deðildir diye hatalar aldýk.
bmp180.begin(); komutunu tanýmlayamadýk.


Daha sonra (#include <SFE_BMP180.h>) Sparkfun BMP180 kütüphanesini kullandýk.
Burda ise daha farklý bi hata ile karþýlaþtýk.
(Sera_Sulama:56:17: error: 'class BMP180' has no member named 'readPressure').
Bu seferde ise begin fonksyonunda ki hata giderilmiþken diðer bir fonksyon 
olan readPressure'ý tanýmlayamadýk.Halbuki iki kütüphanede de bu fonksyonlar
tanýmlýydý.Farklý bi Arduino IDE'si indirip tekrar denedik,Online compile yapan
bi kaç sitede de denememize raðmen bu sorunu aþamadýk.Bu sebeple projemizi 
tamamlayamadýk.