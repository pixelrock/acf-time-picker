# Advanced Custom Fields Time Picker Addon

Addon for Advanced Custom Fields to show a time picker.

All of this work is attibutable to:
[Per Soderlind](https://github.com/soderlind) - [http://soderlind.no](http://soderlind.no)

## Dependencies

1. [Advanced Custom Fields](http://wordpress.org/extend/plugins/advanced-custom-fields/) must be installed.

## Installation

* Find the location of your theme folder
* Make a directory for the addon inside your theme files called `library/php/acf-addons/`
* Copy the contents of this repo into the directory

```
cd `~/sites/wp-content/themes/twentytwelve/` 
mkdir -p library/php/acf-addons
mv ~/Downloads/acf-time-picker library/php/acf-addons/
```

* Edit `functions.php` to include the ACF addon

```
if(function_exists("register_field")) {
  register_field('acf_time_picker', dirname(__FILE__) . '/library/php/acf-addons/acf-time-picker/main.php');
}
```
