# Basic example
Here is simple example you can use to create with this package:

<img width="300" height="300" alt="Loading basic_example.gif ... [6.35MB]" src="https://raw.githubusercontent.com/radnive/Flutter_TextMarquee/main/example/basic_example.gif">

```dart
TextMarquee(
  '"Stay close to anything that makes you glad you are alive." -Hafez',
  spaceSize: 72,
  style: const TextStyle(
    color: Colors.white,
    fontWeight: FontWeight.w600,
    fontSize: 24
  ),
)
```

If you want to use languages whose letters are arranged from right to left (such as Persian), you must set the **rtl** value equal to **true**:

```dart
TextMarquee(
  'به هر چیزی که شما را از اینکه زنده هستید، خوشحال می کند، نزدیک باشید." -حافظ"',
  spaceSize: 72,
  rtl: true,
  style: const TextStyle(
    color: Colors.white,
    fontWeight: FontWeight.w600,
    fontSize: 24
  ),
)
```
