# Colors

## How to Use Colors

### Introduction

The Toolkit comes preloaded with a set of semantic colors allowing project-specific colors to easily be applied to all components of the design system and their states. Each semantic color style has a predefined role to play, it can be customized by changing its HEX values, but it's only possible to change its roles in the design system by creating custom code to support that use case.

E.g., a *Filled* Button uses PrimaryColor as its fill color, while *Elevated* and *Tonal* Buttons use PrimaryColor to fill only their labels. So changing the HEX value of PrimaryColor would impact these buttons (as well as almost every component in the design system).

This can easily be tested and experimented with from the *Getting Started* page of the Toolkit.

![](assets/colors1.png)

> [!CAUTION]
> Colors applied outside the provided color styles will not be in XAML generated via the plugin.

## How to Apply Colors Globally

### Steps

1. **Make sure there is nothing selected**. Using the *Color Styles* panel on the right side of the screen, expand the color drawer.
2. **Right-click on the color and choose edit style**. Or simply hover and click the appearing icon.
   ![](assets/color-edit.png)
3. From the *Properties* section choose the HEX code of the desired color. Close all open panels, by clicking the ✕ icon. You should now see your color updating throughout the document.
   ![](assets/color-edit-properties.png)

> [!TIP]
> It is recommended to do this as the first step of setting up the document. But it can be changed at any time in the future.

> [!CAUTION]
> Changing the color when there's something selected in Figma will only affect the selection itself, not the entire document and the changes won't be exported in XAML.

## How to apply Color to components

1. Select the component from the *Layers* panel in Figma and expand it;
2. Select the layer named `◇ Template/.Templst_[component name]*`;
3. Select the color to change in the *Color Selection* panel on the right-hand side of your monitor;
4. Right-click on the color and choose *Edit Style*;
5. From the Properties section choose the HEX code of the desired color. Close all open panels, by clicking the X.
   ![](assets/colors-apply.png)

** The top layer of a component cannot be colored.*


## How to Change Colors of Component States

Component visual states are usually defined as an extra layer of their main color with varying degrees of opacity, changing the main color will impact all states for all component e.g. changing PrimaryColor would change all state colors for types of Buttons. It is not recommended to customize component states individually as the plugin may not generate proper XAML for this.

### Steps:

1. Select the component from the *Layers* panel in Figma and expand it
2. Update colors to both: `State Layer` AND `◇ Template/.Templst_[component name]`
   ![](assets/colors-update.png)

## How to Generate Color Themes?

Toolkit provides Light and Dark themes that should work for any project. They can be customized to follow to colors required by a particular project. In the case where there is no predefined color theme or simply to help fill in the gaps for an existing color theme, we recommend using a tool like the **Material theme Builder**.

## Dark Mode

The Toolkit design system comes with both light and dark mode color styles. You will need to set the appropriate colors for each theme, considering that each color style name should match between both modes.  (E.g, Light/Primary – Dark/Primary)
 
When running the plugin, users can toggle between light mode and dark mode displays using the dark theme color values that have been set. To get the desired dark mode look, make sure the names of your styles match in both Light and Darth and only the HEX values changes. 

## Preview dark mode in the Plugin

1.	Select your screen and Run the Uno Platform plugin.
2.	Select the Preview Tab and click Refresh.
3.	Set the toggle switch to the Dark theme below your rendered design.

## Designing for dark mode

1.	Edit the HEX values of the Dark theme color styles
2.	Select a screen that uses the light theme
3.	Run Atlas Theme Manager Plugin** and select “Dark” from the drop-down. This will swap all “Light” values with the dark value styles with corresponding names.

More details to get those tools on the [Download & Tools](https://platform.uno/docs/articles/external/figma-docs/download.html) page.
