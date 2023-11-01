---
description: Built-in Types
---

# 🧞 Yerleşik Tipler

Dart'ta konu alcağımız 17 Tip vardır. Gözünüz korktu mu? Korksun çünkü korkutucu. 😂 Sakin sakin açıklaya açıklaya gidelim.

#### Numbers

Double ve Int olmak üzere iki tane sayısal tip vardır. Değişkenlerde bunların örneklerini paylaşmıştık.&#x20;

#### Strings

Yazı tipi veri tipidir. Örneğini değişkenlerde paylaştık. Yazıyı uzatmamak için hızlı geçiyoruz.

#### Booleans

Doğru veya Yanlış. True veya False işte bütün mesele bu. Bunu da değişkenlerde paylaştık.&#x20;

#### Records

Records Dart 3.0 versiyonuyla eklenmiştir. Değişmez, anonim ve toplanmış bir tiptir. Records sabir boyutludur. Kodla daha iyi anlayalım.

```dart
var record = ('first', c : 2, true, 'Püskevit', 10.356);
(String, int) record1 = ('Frappaçino', 124);
```

#### Lists

Listler benzer tipli değişkenleri toplu şekilde tutmamıza yarar. Sıralanmış objeleri tutar. Değişkenler kısmında örnek vardır.

#### Sets

Sıralanmamış benzersiz objeleri barındırır.&#x20;

```dart
var araba = <String>{'ferrari','tofaşk','togg'};
araba.add('s2000');
```

#### Maps

Key ve Value şeklinde değerleri tutarız.

```dart
var sinif = {'1' : 'a', '2' : 'e'};
```

#### Runes

Unicode karakterlerin değişkenlerde tutulabilmesini sağlar. Kütüphane kullanılmalıdır.

```dart
import 'package:characters/characters.dart';

void main() {
  var hi = 'Hi 🇩🇰';
  print(hi);
  print('The end of the string: ${hi.substring(hi.length - 1)}');
  print('The last character: ${hi.characters.last}');
}
```

#### Symbols

Symbols çok kullanılmaz ancak API tanımlamalarında vs kullanılabilir.

```dart
#serverEmre
```

#### Null

Dart null safety bir dildir. Ama aşağıdaki gibi bunu bilerek yaptığınızı derleyiciye soru işareti ile ifade edebilirsiniz.

```dart
int? emre;
```

#### Objects

#### Enum

#### Future

#### Iterable

#### Never

#### dynamic

#### void

