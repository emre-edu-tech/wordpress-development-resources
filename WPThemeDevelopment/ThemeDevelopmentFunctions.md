# Starting Theme Development
Here are the list of some functions that you should definitely need while starting to develop your next Wordpress Theme.
Note: `add_theme_support()` function is also important while developing custom themes but it has its own file so check that file for more information. 
- `get_header()`: Load the header template. If there is a specific header other than the default one. Check the parameters.
- `get_footer()`: Load the footer template. If there is a specific footer other than the default one. Check the parameters.
- `language_attributes()`: Builds HTML attributes containing the text direction and language information for the page. Only valid for html tag.
- `bloginfo()`: Displays information about the current site. Check the possible values for parameter. If it is empty then it echoes the Site Title.
- `wp_head()`: Prints scripts or data in the head tag on the frontend.
- `wp_footer()`: Prints scripts or data before closing body tag on the frontend.