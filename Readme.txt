Biz bu projeyi yaparken kar��la�t���m�z tek sorun k�t�phaneler
ve fonksyonlar�n uyumsuzlu�u oldu.Bas�n� �l��m� i�in Bmp180 
sens�r�n� kulland�k.Bu sens�r i�in ise 2 farkl� k�t�phane kulland�k

�lk ba�ta <Adafruit_BMP085.h> k�t�phanesini kulland���m�zda bu fonksyonlar
k�t�phanenin test kodlar�nda tan�ml� ve �al���yor olmas�na ra�men bu 
fonksyonlar bu k�t�phanede tan�ml� de�ildir diye hatalar ald�k.
bmp180.begin(); komutunu tan�mlayamad�k.


Daha sonra (#include <SFE_BMP180.h>) Sparkfun BMP180 k�t�phanesini kulland�k.
Burda ise daha farkl� bi hata ile kar��la�t�k.
(Sera_Sulama:56:17: error: 'class BMP180' has no member named 'readPressure').
Bu seferde ise begin fonksyonunda ki hata giderilmi�ken di�er bir fonksyon 
olan readPressure'� tan�mlayamad�k.Halbuki iki k�t�phanede de bu fonksyonlar
tan�ml�yd�.Farkl� bi Arduino IDE'si indirip tekrar denedik,Online compile yapan
bi ka� sitede de denememize ra�men bu sorunu a�amad�k.Bu sebeple projemizi 
tamamlayamad�k.