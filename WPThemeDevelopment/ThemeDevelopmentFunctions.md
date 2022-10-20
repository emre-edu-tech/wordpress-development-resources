# Starting Theme Development
Here are the list of some functions that you should definitely need while starting to develop your next Wordpress Theme.
Note: `add_theme_support()` function is also important while developing custom themes but it has its own file so check that file for more information. 
- `get_header()`: Load the header template. If there is a specific header other than the default one. Check the parameters.
- `get_footer()`: Load the footer template. If there is a specific footer other than the default one. Check the parameters.
- `language_attributes()`: Builds HTML attributes containing the text direction and language information for the page. Only valid for html tag.
- `bloginfo()`: Displays information about the current site. Check the possible values for parameter. If it is empty then it echoes the Site Title.
- `wp_head()`: Prints scripts or data in the head tag on the frontend.
- `wp_footer()`: Prints scripts or data before closing body tag on the frontend.
- `body_class()`: Prints the space-separated class names for the body element for every page. If it is wanted to add custom classes to body element, then space-separated class names can be given to the function paramteter and they will be added to default body classes.
- `wp_body_open()`: Triggers after the opening body tag. It is mostly used to add code which is supposed to be added after the opening body tag.
## Functions and hooks that are used when adding styles and scripts to the custom theme
- `wp_enqueue_scripts`: Hook name to enqueue theme styles and scripts. 
- `wp_enqueue_style()`: Register the styles and enqueues them. Check for the different parameters for this function.
- `wp_register_style()`: Registers a stylesheet and make it available to use later using its handle.
- `wp_enqueue_script()`: Register the script and enqueues them. Check for the different parameters for this function.
- `wp_register_script()`: Registers a new script and make it available to use later using its handle.
- `get_template_directory_uri()`: Retrieves the URI(WITHOUT TRAILING SLASH) of the template directory for the active theme.
- `get_template_directory()`: Retrieves absolute template directory path for the active theme. 
- `get_stylesheet_directory_uri()`: Retrieves the URI(WITHOUT TRAILING SLASH) of the stylesheet directory for the active theme.
- `get_stylesheet_uri()`: Retrieves the URI of the stylesheet for the active theme i.e. style.css file.
- `filemtime()`: Returns the last modification time of a file given as a parameter. If the file is not modified since the last modification, then it returns false. This function is generally used for file versioning while development.
- `get_template_part()`: Loads a template part into a template. For different or specialised usage, check the Wordpress documentation.
- `the_custom_logo()`: Displays the custom logo on the frontend that has been added using WP Customizer.
- `has_custom_logo()`: Determines whether the site has custom logo.