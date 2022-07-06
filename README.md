Step #1: Create the folder of Hello World module<br>
```app/code/VendorName/ModuleName```
Step #2: Create etc/module.xml file.
```app/code/VendorName/ModuleName/etc/module.xml```
Step #3: Create etc/registration.php file
```app/code/VendorName/ModuleName/registration.php```
Step #4: Create routes.xml file
```app/code/VendorName/ModuleName/etc/frontend/routes.xml```
Step #5: Create the controller and action
```app/code/VendorName/ModuleName/Controller/Index/Test.php```
Step #6: Run the below Code
``sudo php bin/magento setup:upgrade;
  sudo php bin/magento setup:di:compile;
  sudo php bin/magento cache:flush;``
