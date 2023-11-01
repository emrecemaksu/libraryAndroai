# 🚙 Yavaştan Projemizi Oluşturalım.

Dart ile çalışmak istiyorsak aslında .dart uzantılı bir dosya oluşturup onun içinde çalışmalarımızı yapabiliriz. Ama bu bana yetmez ben proje oluşturup yayınlayıp para kazanacağım mı diyorsunuz. O halde aşağıdaki kodu terminalde projeyi oluşturmak istediğimiz klasörün içinde çalıştıralım.

```
dart create -t console [proje_ismi]
```

Kod ile beraber proje adımız ne ise klasörün içinde artık o isimde bir klasör oluşmuş olacak. Klasörün iç yapısını görmek istersek de aşağıdaki gibi bir durum bizi editörde karşılayacak.

```
emrecemaksu@Emre helloworld % ls
CHANGELOG.md            
README.md               
analysis_options.yaml   
bin                     
lib                     
pubspec.lock            
pubspec.yaml            
test
emrecemaksu@Emre helloworld % cd bin
emrecemaksu@Emre bin % ls
helloworld.dart
emrecemaksu@Emre lib % ls
helloworld.dart
```

Biraz inceleyecek olursak bin klasöründe olan dosyanın içinde main methodunu görürüz. Bu method uygulamamızın başladığı yerdir.&#x20;

```dart
import 'package:helloworld/helloworld.dart' as helloworld;

//Uygulama Ana Method
void main(List<String> arguments) {
  print('Hello world: ${helloworld.calculate()}!');
}
```

Ama diyeceksiniz ki lib klasöründe de aynı isimde dosya var. Dosya isimleri kadar içerik de önemlidir. lib de hesap yapıtğımız Methodumuz mevcut ve mainden bu methodu çağırıp işlemimizi yaptırıyoruz. Tabii ki siz istediğiniz gibi methodları ekleyip özelleştirebilirsiniz.

```dart
int calculate() {
  return 6 * 7;
}
```

Tabii biz bu yazıda uygulama oluşturmayı ele aldığımız için geri kalan şeyler bir başka yazının konusu :smile:
