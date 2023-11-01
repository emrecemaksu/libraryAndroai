---
description: Variables
---

# 👾 Değişkenler

Flutter Variables açısından kolaylatıcı çözümler sunabilmekte. Hadi gelin beraber bu değişkenleri inceleyelim.

```dart
int i = 10; //Tam sayı alır.
double j = 15.5; //Noktalı değer alır.
var k = 'Emre'; //Alınan değere göre int, string, object, double olabilir.
Object o = 'Objem'; //Değişkenler de her şey gibi Objedir!
String s = 'EmreCem'; //Yazı tipidir.
bool isCar = false; //2 değer alır true yada false
```

Dart Null Safety bir dildir. Değişkeni değersiz bırakamazsınız. Ve bunun için programa bunu belitmeniz gerekmektedir. Buna biraz bakalım.

```dart
int? yas; //Değersiz ama böyle bırakmayı sevmiyoruz.
assert(yas = null); //Üretilen code ignore edilir.
```

Late anahtar kelimemiz var. Bu da değişkenin başına gelerek değişkene geç bir atama yapılacağını belirtir.

```dart
late String aciklama;

void main() {
  description = 'Merhaba!';
  print(aciklama);
}

late String sicaklik = okuSicaklik();
//sicaklik okuSicaklik() çağırılmadan kullanılmaz.
```

Final Ve Const anahtar kelimelerimize de bir bakalım. Final (Run Time) çalışma anında değerlendirilirken Const (Compile Time) derleme anında değerlendirilir.

```dart
final name = 'Bob'; // Tipsiz. var gibi düşünün.
final String nickname = 'Bobby';
const bar = 1000000; // Birim basınç (dynes/cm2)
const double atm = 1.01325 * bar; // Standard atmosfer
var foo = const []; //foo ya verilen değer const olan bir list.
final bar = const [];
const baz = []; // Boş Baz listesi const
foo = [1, 2, 3]; // foo değer alabildi.
//baz = [42]; baz const olduğu için değer alamaz.
const list = [i as int]; // typecast şeklinde kullanalım.
const map = {if (i is int) i: 'int'}; // is ve collection if olarak kullanımı
const set = {if (list is List<int>) ...list}; // set yapısının yayılması
```

Kafanız çok karışırsa yaparak öğrenirsiniz. Teoride takılır kalmayın :thumbsup:
