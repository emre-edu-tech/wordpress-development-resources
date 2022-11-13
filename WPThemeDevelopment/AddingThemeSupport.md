# Theme Functionality
## Adding Theme Support
Adding theme support is one of the most important parts of theme development. `add_theme_support()` is the function that needs to be used to **register theme support for a given feature**.
### Possible parameter values
- `add_theme_support('title-tag')`: This is the Wordpress recommended way of adding title tag to a Wordpress website. Remember to delete the hard-coded title tag after adding this theme support.
- `add_theme_support('custom-logo', [$defaults_arr])`: Enables a custom logo in theme.
    -   $defaults_arr
        `'height'               => 100,`
        `'width'                => 400,`
        `'flex-height'          => true,`
        `'flex-width'           => true,`
        `'header-text'          => array( 'site-title', 'site-description' ),`
        `'unlink-homepage-logo' => true,`
- `add_theme_support('custom-background', [$defaults_arr])`: Enables a custom background in theme.
    -   $defaults_arr
        `'default-color'      => '0000ff',`
        `'default-image'      => get_template_directory_uri() . '/images/wapuu.jpg',`
        `'default-position-x' => 'right',`
        `'default-position-y' => 'top',`
        `'default-repeat'     => 'no-repeat',`
- `add_theme_support('post-thumbnails')`: Post types will have the support for the featured image.
- `add_theme_support('customize-selective-refresh-widgets')`: Customizer window will refresh just for the necessary part of the preview window for the widgets.
- `add_theme_support('automatic-feed-links')`: Gives the possibility to RSS readers to find the website post updates.
- `add_theme_support('html5, ['search-form', 'comment-form', 'comment-list', 'gallery', 'caption', 'script', 'style'])`: Allows the use of HTML5 markup.
- `add_editor_style()`: Allows theme developers to link a custom stylesheet file to the TinyMCE visual editor. The default stylesheet is editor-style.css
- `add_theme_support('wp-block-styles')`: Useful to load your styles for the Gutenberg editor screen
- `add_theme_support('align-wide')`: Gives the option for some of the Gutenberg blocks to be aligned as wide and full width