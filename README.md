# ZR CKE5 Recipe Installation Guide

To install the ZR CKE5 Recipe, follow the steps below:

1. Ensure the below has been added to the `composer.json` **installer-paths**:
    ```sh
    "web/recipes/custom/{$name}": ["type:drupal-recipe"]
    ```
2. Run `composer require zr/zr-cke5-recipe`
3. Run the following command (within `/web` directory):

    ```sh
    ddev drush recipe recipes/custom/zr-cke5-recipe
    ddev drush cim --partial --source=recipes/custom/zr-cke5-recipe/config -y
    ```

This command will execute the ZR CKE5 Recipe installation.
