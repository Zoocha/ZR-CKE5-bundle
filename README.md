# Zoocha CKE5 Recipe Installation Guide

To install the Zoocha CKE5 Recipe, follow the steps below:

1. Open your terminal.
2. Navigate to your project directory. 
3. Add the below in the Drupal Root's composer.json installer-paths
```sh
"web/recipes/custom/{$name}": ["type:drupal-recipe"]
```
4. Run the following command:

    ```sh
    ddev drush cdel editor.editor.basic_html
    ddev drush cdel editor.editor.full_html
    ddev drush cr
    ddev drush recipe recipes/custom/zoocha-cke5-recipe
    ```

This command will execute the Zoocha CKE5 Recipe installation.