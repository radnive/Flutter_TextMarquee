# Text marquee

<p>
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/github/license/radnive/flutter_textMarquee?logo=github" />
  </a>
  <a href="https://pub.dev/packages/text_marquee/changelog">
    <img src="https://img.shields.io/badge/version-0.0.1-blueviolet" />
  </a>
  <a href="https://docs.flutter.dev/development/tools/sdk/releases">
    <img src="https://img.shields.io/badge/flutter-2.17.5-blue" />
  </a>
  <a href="https://dart.dev/guides/whats-new">
    <img src="https://img.shields.io/badge/dart-2.16.2-blue" />
  </a>
</p>

Open source flutter package, Text marquee for flutter apps.

# Getting Started
- [Installing](#installing)
- [Basic Example](#basic-example)
- [Parameters description](#parameters-description)

# Installing
Add this line to the **pubspec.yaml** file below the dependencies:
```yaml
dependencies:
  text_marquee: ^0.0.1
```

Now to use, import this package into the desired file as follows:
```dart
import 'package:text_marquee/text_marquee.dart';
```

# Basic example
Here is simple example you can use to create with this package:

<img width="300" height="300" alt="Loading basic_example.gif ... [6.35MB]" src="https://raw.githubusercontent.com/radnive/Flutter_TextMarquee/main/example/basic_example.gif">

```dart
TextMarquee(
  '"Stay close to anything that makes you glad you are alive." -Hafez',
  style: Types.of(context).headline5!.copyWith(
    color: Colors.white,
    fontWeight: FontWeight.w600,
  ),
  spaceSize: 72
)
```

If you want to use languages whose letters are arranged from right to left (such as Persian), you must set the **rtl** value equal to **true**:

```dart
TextMarquee(
  'به هر چیزی که شما را از اینکه زنده هستید، خوشحال می کند، نزدیک باشید." -حافظ"',
  style: Types.of(context).headline5!.copyWith(
    color: Colors.white,
    fontWeight: FontWeight.w600
  ),
  spaceSize: 72,
  rtl: true
)
```

# Parameters description
|Parameter|Default|Description|
|---------|-------|-----------|
|**text** <br>*String*||Text to be scrolled.|
|**style** <br>*TextStyle*|TextStyle()|Text style.|
|**duration** <br>*Duration?*|null|Animation duration.|
|**curve** <br>*Curve*|Curves.linear|Animation curve.|
|**delay** <br>*Duration*|Duration(seconds: 2)|Delay time for scrolling start.|
|**spaceSize** <br>*double*|32|The distance between the original text and its subsequent repetition.|
|**startPaddingSize** <br>*double*|0|Text spacing from the beginning of the widget.|
|**rtl** <br>*bool*|false|If the text is arranged from the right, it should have a value of True.|
