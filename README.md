
# Avro Phonetic TextField

A Flutter package that provides a custom `TextField` widget with Bangla phonetic typing support. English characters are automatically transliterated into Bangla upon pressing the space key. Users can toggle between Bangla and English typing modes using `Ctrl + M`.

## Features

- **Bangla Phonetic Typing**: Type in English, and the text will be transliterated to Bangla.
- **Toggle Language Mode**: Switch between Bangla and English using Ctrl + M.
- **Fully Customizable**: Supports all properties of Flutter's built-in TextField, except for the controller, which is internally managed.
- **Real-Time Transliteration**: The transliteration is applied when the space key is pressed.

## Installation

Add the following to your `pubspec.yaml`:
```yaml
dependencies:
    avro_phonetic_textfield: latest_version
```

Then, run:
```shell
flutter pub get
```

## Usage
```dart
// import the package
import 'package:avro_phonetic_textfield/avro_phonetic_textfield.dart';

// anywhere in the app
AvroPhoneticTextField(
    decoration: InputDecoration(
        labelText: 'Type in Bangla',
        border: OutlineInputBorder(),
    ),
    maxLines: 1,
    style: TextStyle(fontSize: 18),
    keyboardType: TextInputType.text,
    textAlign: TextAlign.start,
)
```

## Properties

AvroPhoneticTextField supports all properties of Flutter’s built-in TextField, except `controller`, which is internally managed.


## How It Works
- Type in English characters (e.g., ami → আমি).
- Press space to trigger transliteration.
- Use Ctrl + M to switch between Bangla and English modes.

## License
The Unlicense
