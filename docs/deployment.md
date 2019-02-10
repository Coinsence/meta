# Deployment

## HumHub

### Humhub installation 

Follow instructions of a regular HumHub [Installation & Administration](http://docs.humhub.org/admin-README.html)

Humhub version updates can be done directly via Humhub administration UI 

### Coinsence modules integration 

Besides standalone humhub modules, we're creating new modules or working around already existing ones, in order to install them you can clone them from [Coinsence repoisotry](https://github.com/Coinsence) directly under *protected/humhub/modules* or for a best code separation you may clone them into an External Modules Directory outside the default HumHub modules and then configuring autoload paths for these modules by changing the following file **protected/config/common.php** : 

```php
return [
    'params' => [
        'moduleAutoloadPaths' => ['path/to/your/modules/folder'],        
    ],
]
```

