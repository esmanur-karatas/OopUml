# OopUml
Bu depo, nesne yönelimli programlama konusunda oluşturduğum UML diyagramlarını içermektedir. Nesne yönelimli programlama prensiplerini açıklamak ve görselleştirmek için oluşturulan UML diyagramları, sınıf yapıları, kalıtım ilişkileri, arayüzler ve diğer nesne yönelimli kavramları içerir. Bu diyagramlar, OOP prensiplerini anlamak ve öğrenmek isteyenler için yararlı bir kaynak olmayı amaçlamaktadır. Umuyorum ki, bu diyagramlarla nesne yönelimli programlamayı daha iyi anlayabilir ve projelerinizde bu prensipleri uygulamak için bir rehber olarak kullanabilirsiniz. Katkılarınız ve geri bildirimleriniz her zaman açıktır, böylece bu depoyu daha da geliştirebiliriz

=====================================================================
Hayvanat Bahçesi Yönetim Sistemi - Polimorfizm Modeli

Bu UML sınıf diyagramı, bir hayvanat bahçesindeki hayvanların bilgilerini takip etmek için tasarlanan bir sistem üzerinde polimorfizm modelini gösterir. Polimorfizm, farklı hayvan grupları için aynı işlevleri farklı şekilde gerçekleştirme yeteneğidir.

Sınıflar:
1. Hayvan: Bu temel sınıf, hayvanların genel özelliklerini tanımlar ve tür adı, ağırlık, yaş gibi ortak özelliklere sahiptir.
   - +türAdı: String
   - +ağırlık: double
   - +yaş: int
   +getDosage(): String (Polimorfik metod, farklı hayvan grupları için ilaç dozajını döndürür)
   +getFeedSchedule(): String (Polimorfik metod, farklı hayvan grupları için yem verme zamanlarını döndürür)

2. Atlar: Hayvan sınıfından türetilen bu sınıf, atlar, zebralar, eşekler gibi atgilleri temsil eder.
   - +getDosage(): String (Atlar için ilaç dozajı hesaplama)
   - +getFeedSchedule(): String (Atlar için yem verme zamanları hesaplama)

3. Kedigiller: Hayvan sınıfından türetilen bu sınıf, kaplanlar, aslanlar gibi kedigilleri temsil eder.
   - +getDosage(): String (Kedigiller için ilaç dozajı hesaplama)
   - +getFeedSchedule(): String (Kedigiller için yem verme zamanları hesaplama)

4. Kemirgenler: Hayvan sınıfından türetilen bu sınıf, sıçanlar, kunduzlar gibi kemirgenleri temsil eder.
   - +getDosage(): String (Kemirgenler için ilaç dozajı hesaplama)
   - +getFeedSchedule(): String (Kemirgenler için yem verme zamanları hesaplama)

Sınıf diyagramı, Hayvan sınıfından türetilen Atlar, Kedigiller ve Kemirgenler sınıflarını gösterir. Polimorfizm sayesinde, her alt sınıf kendi getDosage() ve getFeedSchedule() metodlarını farklı şekilde uygular ve hayvan gruplarına özgü işlevselliği sağlar.

Bu sınıf diyagramı, hayvanat bahçesi yönetim sisteminin temel tasarımını gösterir ve farklı hayvan grupları için esnek ve genişletilebilir bir yapı sunar. Her hayvan grubu için özel işlemler yapmak için uygun bir temel sağlar.

Katkılarınız ve geri bildirimleriniz her zaman açıktır, böylece programı daha da geliştirebiliriz.

İyi kullanımlar!

===============================================================
Üniversite Yönetim Sistemi - Class (Sınıf) Diyagramı

Bu Class (Sınıf) diyagramı, bir üniversite yönetim sisteminin temel yapılarını gösterir. Üniversiteye ait sınıflıklar, çalışma ofisleri ve departmanlar ile çalışanlar arasındaki ilişkileri gösterir.

Sınıflar:
- Üniversite: Bu sınıf üniversiteyi temsil eder ve sınıflıklar, çalışma ofisleri ve departmanlar ile ilişkilidir.
- Sınıflık: Üniversiteye ait sınıflıkları temsil eder ve departmanlara ait ofisler ile ilişkilidir.
- Çalışma Ofisi: Departmanlara ait ofisleri temsil eder.
- Departman: Üniversiteye ait departmanları temsil eder ve çalışanlar ile ilişkilidir.
- Çalışan: Bu sınıf, üniversitede çalışanları temsil eder ve profesör veya memur olabilir. Her çalışan bir ofiste çalışır.

İlişkiler:
- Üniversite sınıfı, Sınıflık, Çalışma Ofisi ve Departman sınıfları ile ilişkilidir.
- Sınıflık sınıfı, Departman ve Çalışma Ofisi sınıfları ile ilişkilidir.
- Çalışma Ofisi sınıfı, Departman sınıfı ile ilişkilidir.
- Departman sınıfı, Çalışan sınıfı ile ilişkilidir.
- Çalışan sınıfı, Çalışma Ofisi sınıfı ile ilişkilidir.

Bu Class (Sınıf) diyagramı, üniversite yönetim sisteminin temel yapılarını ve bu yapılar arasındaki ilişkileri gösterir. Sistemde yer alan sınıflar ve ilişkiler, üniversitedeki sınıflıklar, ofisler, departmanlar ve çalışanlar arasındaki ilişkileri modellemek için kullanılır.

Katkılarınız ve geri bildirimleriniz her zaman açıktır, böylece programı daha da geliştirebiliriz.

İyi kullanımlar!
