# DataFeedWatch Connector

This module has been deprecated in favour of the newer version.

### Where to find the newer version of the module?

The new version of the module is available here: https://packagist.org/packages/datafeedwatch/dfwconnector-magento2

### How to migrate to a newer version?

1. You fill first need to SSH into the machine that is running your Magento shop. 
2. After login go to Magento home directory.
3. Ensure that Composer is installed, by checking which version you have:
    ```
   composer --version
    ```
4. Inside the Magento Home uninstall the module
   ```
   composer remove datafeedwatch/connector
   ```
5. Finally clean up tasks:
   ```
   bin/magento setup:upgrade
   bin/magento cache:clean
   bin/magento setup:di:compile
   ```
6. Follow the guide to install the new version of the module available here: https://packagist.org/packages/datafeedwatch/dfwconnector-magento2  
7. You access tokens won't change and there is no need to update anything id DataFeedWatch.