# Shopify Theme Downloader

Download a complete copy of a Shopify theme via command line. This tool will download all theme assets exactly as they exist on the shop, and also compress them into a TAR archive.

Note: No unit tests are provided for this yet.

## Installation

You can either clone this repository, or more easily, download the PHAR archive located in `build` directory of this repository.

## Usage

*Below assumes usage of the PHAR archive*

```php theme-download.phar <shop> <api> <theme>```

Example:

```php theme-download.phar my-cool-shop some-api-key:some-api-password 123456789```

## Output

Will download a complete directory, as well it will create a TAR archive of that directory.

```conf
php theme-download.phar download demo-shop ecd80185b409eeb38b03597a3956543:551f5a55f7f061a370304cca668646b7 32480591923
Total assets: 46
[1/46] 0% | assets/favicon.png | Downloaded
[2/46] 0% | assets/favicon.svg | Downloaded
[3/46] 1% | assets/image-page-legal.jpg | Downloaded
# ...
Completed download, demo-shop-32480591923.tar is available
```
