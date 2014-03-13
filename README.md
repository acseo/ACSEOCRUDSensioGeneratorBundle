# ACSEO CRUD Generator using SensioGeneratorBundle

This bundle provide Twig template to generate CRUD applications with SensioGeneratorBundle in your Symfony2 application

## Requirements
- A Symfony 2 Project with SensioGeneratorBundle (embeded by default in the Symfony Standard Distribution)
- BraincraftBootstrapBundle (https://github.com/braincrafted/bootstrap-bundle)
- ACSEO ApyDataGridBundle (https://github.com/acseo/APYDataGridBundle)
- ACSEO FastShowGeneratorBundle (https://github.com/acseo/FastShowGeneratorBundle)

## How to use it

### Step 1 : Get the code
Get the code using ``git submodule`` command :
````
cd /path/to/my/sf2project
git submodule add https://github.com/acseo/ACSEOCRUDSensioGeneratorBundle app/Resources/SensioGeneratorBundle
```` 
Now you should see a directory called 'skeleton' in app/Resources/SensioGeneratorBundle

### Step 2 : Generate the CRUD for an Entity
CRUD creation is just the same as the original ``app/console doctrine:generate:crud`` command.

````
 cd /path/to/my/sf2project
php app/console doctrine:generate:crud
````
And follow the guidelines.
All the crud stuff, configured to work with Bootstrap 3, APYDataGrid and FastShow should be generated now ! 

**But we must configure some things**

### Step 3 : Configure the grid

You will see that ``TODO`` insctruction have been generated in your Controller.
For now, we are not able to generate some usefull code to describe the attributes that the POST and PUT methods are waiting for.

Simply edit your Controller file to make it work as you expect.