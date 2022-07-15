# Starting a New Design and General Tips

To ensure having the proper XAML and previews from the plugin, please follow these guidelines:

1. Duplicate the Uno Platform Material Toolkit, which can be found [here](../../download.md). First, rename it and change the cover image then **work from the provided file**. Do not copy-paste elements from the toolkit into your own files as the plugin does not support your existing design files.

   > [!IMPORTANT]
   > **Do not use the Uno Toolkit as a Figma Library linked to a new file nor to an existing Figma file**. Referenced components and styles will not render proper code from a new file and some advanced features won't be available. Always start working within the provided file.
   
2. **Use the provided Color Styles**. Follow the *Getting Started Instructions* provided with the Toolkit to learn how to update the HEX values of the included semantic color styles.

3. **Use the provided Type Styles**. Uno Toolkit does not currently support custom fonts, nor custom sizes. Custom fonts can be included in designs, of course, but the XAML for these will not be generated on export. You can, however, change the default font for Uno Material by following [this guide](/docs/articles/external/uno.themes/doc/material-getting-started.html#change-default-font), and it will be applied to all Uno Material or Uno Toolkit control styles.

4. **Use Page Templates**. Uno Toolkit provides handy templates that include all the proper layer structures to generate the XAML and have a preview of the designs through the plugin. Just pick the template you need from the *Assets* section in Figma, drag it to the work canvas, and *Detach the instance* to have a fully functional page ready to work with. **Page instances must always be detached from their Template Masters** to function properly with the *Uno* *Toolkit*.

5. **Always use Auto layouts** for optimal rendering when placing components into your layouts. The same also applies when using custom components or layouts. Toolkit rendering does not support elements positioned with absolute (*X,Y*) coordinates.


## Links

Duplicate the Uno Platform Material Toolkit and install the plugin from the [download](../../download.md) page.
