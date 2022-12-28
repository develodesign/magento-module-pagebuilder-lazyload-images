# Magento 2 Module for adding loading="lazy" to page builder images
 
 - [Main Functionalities](#markdown-header-main-functionalities)
 - [Installation](#markdown-header-installation)
 - [Configuration](#markdown-header-configuration)


## Main Functionalities
Uses the modern browser loading="lazy" attribute on images added via page builder. Can be turned on and off per image as needed.


* **Do not turn on for images loaded above the fold, this causes unnecessary layout shift (CLS).**


### Composer

 ```
 composer require develodesign/magento-module-pagebuilder-lazyload-images

 bin/magento module:enable Develodesign_PagebuilderLazyLoadImages
 bin/magento setup:upgrade
 bin/magento cache:flush
```

### Zip file

 - Unzip the zip file in `app/code/Develodesign/PagebuilderLazyloadImages`
 - Enable the module by running `php bin/magento module:enable Develodesign_PagebuilderLazyloadImages`
 - Apply database updates by running `php bin/magento setup:upgrade`\*
 - Flush the cache by running `php bin/magento cache:flush`

## Installation
  * = in production please use the option `--keep-generated` 
