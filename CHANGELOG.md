# Changelog

## [1.0.0] - 2025-01-29
- Initial release of the package.
- Added support for Bangla phonetic typing.
- Implemented real-time transliteration when space key is pressed.
- Added language mode toggle (Bangla and English) using `Ctrl + M`.
- Fully customizable with all properties of Flutter's built-in `TextField` except the `controller`.
- Added installation and usage instructions.

## [1.0.1] - 2025-01-29
- added support for on screen keyboards by changing the implementation
- using `event.logicalKey.keyLabel` instead of `event.character`