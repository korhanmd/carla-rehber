# Carla Simulator Kurulum Rehberi

---

## Gerekli Dosyalar

İlk olarak Carla'nın derlenmiş sürümleri indirilir. Bu işlem aşağıdaki bağlantılardan yapılır. Daha sonra indirilen sıkıştırılmış dosyanın içindekiler çıkarılır.

#### Ubuntu için:

[CARLA_0.9.6.tar.gz](https://github.com/carla-simulator/carla/releases/tag/0.9.6) dosyası indirilir.

#### Windows için:

[CARLA_0.9.5.zip](https://github.com/carla-simulator/carla/releases/tag/0.9.5) dosyası indirilir.

---

## Anaconda Ortamını Hazırlama

Simülatörün kodlarını çalıştırabilmek için Anaconda Prompt'ta `conda create -n carla python=3.7` komutu ile yeni bir ortam oluşturulur ve `activate carla` komutu ile aktif edilir. `pip install pygame` ve `conda install -c anaconda numpy` komutları ile gerekli kütüphaneler kurulur

---

## Simülatörü Manual Modda Çalıştırma

Ubuntu'da `./CarlaUE4.sh`, Windows'ta `CarlaUE4.exe` çalıştırılarak simülatör başlatılır. Anaconda Prompt'ta Carla'nın dosyalarının olduğu klasörün altında `PythonAPI/examples` konumuna gidilir. Burada `python spawn_npc.py -n 10` komutu ile 10 adet araç simülatörde rastgele oluşturulur. Komuttaki 10 sayısı değiştirilerek farklı sayıda araç simülatörde başlatılabilir. Araçlar simülatörde oluştuktan sonra `python manuel_control.py` komutu ile manual mod başlatılır.