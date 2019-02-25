# PWA module for SilverStripe

This module will add a Service Worker & Web Manifest to your SilverStripe Project. You can change the PWA settings in the settings section inside the CMS.

## Requirements
- SilverStripe ^4.0
- silverware/colorpicker ^1.0
- silverstripe/vendor-plugin ^1.0

## Installation

```
composer require mdiederen/SilverStripe-PWA
```

## Usage

- Run dev/build after the installation.
- Include the js to register the Service Worker
```
Requirements::javascript('mdiederen/SilverStripe-PWA:resources/js/registerServiceWorker.js');
```
- Add this metadata to the header of the website
```
<meta name="theme-color" content="$SiteConfig.ManifestColor">
<link rel="manifest" href="{$BaseHref}manifest.json">
```
## License

See [License](LICENSE)

## Maintainers

Michiel Diederen - michiel@violet88.nl