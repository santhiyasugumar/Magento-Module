Step #1: Create the folder of Hello World module<br>
```app/code/VendorName/ModuleName```<br>
Step #2: Create etc/module.xml file.<br>
```app/code/VendorName/ModuleName/etc/module.xml```<br>
Step #3: Create etc/registration.php file<br>
```app/code/VendorName/ModuleName/registration.php```<br>
Step #4: Create routes.xml file<br>
```app/code/VendorName/ModuleName/etc/frontend/routes.xml```<br>
Here You defining the first part of the route, the URL will be displayed as:<br>
```http://<yourhost.com>/helloworld/*```<br>
Step #5: Create the controller and action<br>
```app/code/VendorName/ModuleName/Controller/Index/Test.php```<br>
Step #6: Run the below Code<br>
````
sudo php bin/magento setup:upgrade;
sudo php bin/magento setup:di:compile;
sudo php bin/magento cache:flush;
````
Route’s in magento are divided into 3 parts: Route frontname, controller and action as following example:<br>
```frontname/controller/action```<br><br>
Your URL now should be as:<br>
````
http://<yourhost.com>/helloworld/index/test
````
