# WordCamp Kansai 2016 Site Design

## File list

### CSS Files
* css/wck2016_main.css
* css/wck2016_teaser.css

### SASS Files
* scss/wck2016_main.scss
* scss/wck2016_teaser.scss

##How to use this files
### For contributor steps
1. Install theme "twenty-sixteen" to your WordPress site
2. Create child theme directory "site-design"
3. Clone this repository to "site-design" directory
4. Create style.css to "site-design" directory and write the following code in style.css

####style.css
      /*
     Theme Name:   WordCamp Kansai 2016 main site.
     Theme URI:    https://github.com/wckansai2016/site-design
     Description:  This theme is WordCamp Kansai 2016 original design.
     Author:       WordCamp Kansai Organizers
     Author URI:   https://2016.kansai.wordcamp.org
     Template:     twentysixteen
     Version:      1.0.0
     License:      GNU General Public License v2 or later
     License URI:  http://www.gnu.org/licenses/gpl-2.0.html
     Text Domain:  wck2016-main
    */

6. Create functions.php and write and write the following code in functions.php

#### functions.php
##### For main site
    add_action( 'wp_enqueue_scripts', 'theme_enqueue_styles' );
    function theme_enqueue_styles() {
        wp_enqueue_style( 'parent-style', get_template_directory_uri() . '/style.css' );
        wp_enqueue_style( 'child-style',
            get_stylesheet_directory_uri() . '/css/wck2016_main.css',
            array('parent-style')
        );
    }

##### For teaser site
    add_action( 'wp_enqueue_scripts', 'theme_enqueue_styles' );
    function theme_enqueue_styles() {
        wp_enqueue_style( 'parent-style', get_template_directory_uri() . '/style.css' );
        wp_enqueue_style( 'child-style',
            get_stylesheet_directory_uri() . '/css/wck2016_teaser.css',
            array('parent-style')
        );
    }

6. Activate this child theme.
7. Enjoy development!

### For organizer steps
1. Login your wordcamp site
2. Activate Jetpack function "Remote CSS"
3. Access menu "Appearance" -> "Remote CSS"
4. Input the following css path to text field "Remote CSS file"

##### For main site
    https://github.com/wckansai2016/site-design/blob/master/css/wck2016_main.css

##### For teaser site
    https://github.com/wckansai2016/site-design/blob/master/css/wck2016_teaser.css

5. Push save button
6. Update field, and display path of Github is converted to the path of the API automatically
7. Design to your site is reflected!
