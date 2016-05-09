# WordCamp Kansai 2016 Site Design

## File list
### CSS Files
* wck2016_main.css
* wck2016_teaser.css
### SASS Files
* wck2016_main.scss
* wck2016_teaser.scss
####include files (for wck2016_main)
Coming soon.

##How to use this files
### Steps
1. Install theme "twenty-sixteen" to your WordPress site
2. Create child theme directory "site-design"
3. Clone this repository to "site-design" directory
4. Create style.css to "site-design" directory
5. Write the following code in style.css

#### Common
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
#### for main site
    @import "css/wck2016_main.css";
#### for teaser site
    @import "css/wck2016_teaser.css";

6. Activate this child theme.
7. Enjoy development!
