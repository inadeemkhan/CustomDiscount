# Mage2 Module Magelumen CustomDiscount

    ``magelumen/module-customdiscount``

 - [Main Functionalities](#markdown-header-main-functionalities)
 - [Installation](#markdown-header-installation)
 - [Configuration](#markdown-header-configuration)
 - [Specifications](#markdown-header-specifications)
 - [Attributes](#markdown-header-attributes)


## Main Functionalities
To Apply custom discount at Cart and Checkout Page.

## Installation
\* = in production please use the `--keep-generated` option

### Type 1: Zip file

 - Unzip the zip file in `app/code/Magelumen`
 - Enable the module by running `php bin/magento module:enable Magelumen_CustomDiscount`
 - Apply database updates by running `php bin/magento setup:upgrade`\*
 - Flush the cache by running `php bin/magento cache:flush`

### Type 2: Composer

 - Make the module available in a composer repository for example:
    - private repository `repo.magento.com`
    - public repository `packagist.org`
    - public github repository as vcs
 - Add the composer repository to the configuration by running `composer config repositories.repo.magento.com composer https://repo.magento.com/`
 - Install the module composer by running `composer require magelumen/module-customdiscount`
 - enable the module by running `php bin/magento module:enable Magelumen_CustomDiscount`
 - apply database updates by running `php bin/magento setup:upgrade`\*
 - Flush the cache by running `php bin/magento cache:flush`


## Configuration

 - isenable (custom_dicount/discount/isenable)


## Specifications

 - Helper
	- Magelumen\CustomDiscount\Helper\Data

 - Observer
	- sales_order_save_after > Magelumen\CustomDiscount\Observer\Frontend\Sales\OrderSaveAfter


## Attributes



