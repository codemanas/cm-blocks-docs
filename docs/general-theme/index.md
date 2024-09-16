Additional CSS refers to custom CSS code that you can add to your website to modify its appearance and behavior beyond what is already provided by your theme or plugins. 
It provides a way to tailor the styling of your website without directly editing the theme's core files, which helps in maintaining the integrity of the theme and simplifies future updates.

## How to add Additional CSS

1. Visit your site’s dashboard. 
2. Navigate to Appearance → Editor. 
3. Click Styles in the Design menu on the left.
    - If your theme includes Style Variations, you must then click the pencil icon to open the Styles options:
         ![Additional CSS To Global Styles](img/custom-css-to-global-styles.png)
4. Click the three dots to the right of the “Styles” heading and choose “Additional CSS“:
![Access Styles Additional Css](img/access-styles-additional-css.png)
5. Type or paste your CSS into the text box provided. 
6. Click the “Save” button at the top right of the screen to save the CSS to your site.


## How to add hover state for navigation block

By default, the new Site Editor doesn't offer an option to set the hover state for navigation items. Therefore, custom CSS is required. Follow the guide on [How to add Additional CSS](#how-to-add-additional-css).

To modify the hover state of every navigation item on your site, use the following CSS:

```css
.wp-block-navigation-item:hover {
    color: #0000FF;
}
```

If you want to apply CSS specifically to the navigation, add a custom class to the navigation block as shown in the screenshot below and adjust your CSS accordingly:

![Specific Header Navigation Hover](img/specific-nav-class-hover.png)

Here's the CSS to target the header navigation:

```css
.your-custom-class .wp-block-navigation-item:hover {
    color: #0000FF;
}
```