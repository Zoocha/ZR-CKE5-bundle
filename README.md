# Zoocha CKE5 Recipe Installation Guide

To install the Zoocha CKE5 Recipe, follow the steps below:

1. Open your terminal.
2. Navigate to your project directory. 
3. Before the recipe installation, run the following composer commands to install the required modules:

    ```sh
    composer require drupal/editor_advanced_link drupal/ckeditor5_plugin_pack
    ```
4. Run the following command:

    ```sh
    drush cdel editor.editor.basic_html
    drush cdel editor.editor.full_html
    drush cr
    drush recipe recipes/custom/zoocha-cke5-recipe
    ```

This command will execute the Zoocha CKE5 Recipe installation.