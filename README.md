# DataFeedWatch Connector

This module has been deprecated in favour of the newer version.

### Where to find the newer version of the module?

The new version of the module is available here: https://packagist.org/packages/datafeedwatch/dfwconnector-magento2

### How to migrate to a newer version?

1. First, log into the machine running your Magento shop via SSH. 
2. Then, go to the Magento home directory.
3. Ensure the Composer is installed. To verify it, check which version you have:
    ```
   composer --version
    ```
4. Uninstall the module:
   ```
   composer remove datafeedwatch/connector
   ```
5. Finally, the clean up tasks:
   ```
   bin/magento setup:upgrade
   bin/magento cache:clean
   bin/magento setup:di:compile
   ```
6. Once completed, follow the guidelines to install the new version of the module available here: https://packagist.org/packages/datafeedwatch/dfwconnector-magento2  
7. Your access tokens won’t change. Therefore, you don’t need to update anything in DataFeedWatch.