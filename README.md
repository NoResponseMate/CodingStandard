<h1 align="center">
    Coding Standard
</h1>

:1st_place_medal: Battle-tested coding standard configuration used in Sylius.

Installation & usage
--------------------

1. Install this package:

    ```bash
    $ composer require --dev sylius-labs/coding-standard
    ```
    
2. Import the configuration file in your `ecs.php`:

    ```php
    $containerConfigurator->import('vendor/sylius-labs/coding-standard/ecs.php');
    ```
   
Example config (ecs.php)
------------------------

    ```php
    use Symfony\Component\DependencyInjection\Loader\Configurator\ContainerConfigurator;
   
    return static function (ContainerConfigurator $containerConfigurator): void {
        $containerConfigurator->import('vendor/sylius-labs/coding-standard/ecs.php');
    };
    ```

Upgrade from YML to PHP config file
-----------------------------------

Use this [package](https://github.com/symplify/config-transformer) and follow their guidelines
to automatically migrate your YML config to a PHP config file.
