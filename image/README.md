# barcode_image

Barcode generation library for Dart that can generate barcodes using the [pub:image](https://pub.dev/packages/image) library.

```dart
// Create an image
final image = Image(300, 120);

// Fill it with a solid color (white)
fill(image, getColor(255, 255, 255));

// Draw the barcode
drawBarcode(image, Barcode.code128(), 'Test', font: arial_24);

// Save the image
File('test.png').writeAsBytesSync(encodePng(image));
```

<img alt="Barcode" src="https://raw.githubusercontent.com/DavBfr/dart_barcode/master/img/test.png">