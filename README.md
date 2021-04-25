# Plugin providing memory plugin loading in Kirikiri

This plugin replaces the plugin loading functionality with one that does not require usage of temporary files in Kirikiri2 / 吉里吉里2 / KirikiriZ / 吉里吉里Z  
Additionally, for Kirikiri2, this will allow usage of the Unicode functions for loading plugins.  

## Building

After cloning submodules, a simple `make` will generate `krmemplugin.dll`.

## How to use

After `Plugins.link("krmemplugin.dll");global.Plugins.prepare_krmemplugin();` is used, the `link`, `unlink`, and `getList` functions will be exposed under the `Plugins` class.

## Limitations

* Susie archive and image plugins are not supported.  
* Unlinking is stubbed.  

## License

This project is licensed under the MIT license. Please read the `LICENSE` file for more information.
