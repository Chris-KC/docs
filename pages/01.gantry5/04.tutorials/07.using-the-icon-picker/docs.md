---
title: Using the Icon Picker
taxonomy:
    category: docs
    tag: [gantry5]
---

Gantry 5 has support for [Font Awesome’s](http://fortawesome.github.io/Font-Awesome/) growing icon library built right into its core. This means that anyone using a Gantry-powered template will have the ability to use any of these incredible vector icons anywhere on your page.

![Icon Picker](icon_picker_2.png?classes=shadow,border)

These serve as lightweight alternatives to image files, can add a visual element to a menu option or an eye-catching accent to a block of text. You can add them to Particles, as well as to fields in your theme's **Styles** administrative panel to add an easily-configured element to your site.

## Using the Icon Picker

[ui-callout]
[ui-callout-item title="Search" position="4%, 2%, se"]
Use this field to search for a icon by name. The number in the upper-right corner of the field indicates how many matches there are to your current string.
[/ui-callout-item]
[ui-callout-item title="Fixed Width" position="4%, 46%, se"]
Selecting this checkbox gives the icon Font Awesome's included `fa-fw` class, setting it as a fixed width. This is useful when different icon widths throw off alignment. It is especially useful in things like navigation lists and list groups.
[/ui-callout-item]
[ui-callout-item title="Spinning" position="4%, 59%, se"]
Selecting this checkbox sets the `fa-spin` class on the icon, causing it to take on an animated spinning effect. Great for circle, cog, and spinner icons.
[/ui-callout-item]
[ui-callout-item title="Size" position="4%, 70%, se"]
This dropdown sets the size of the icon. The options are: Large, 2x, 3x, 4x, and 5x.
[/ui-callout-item]
[ui-callout-item title="Rotation" position="4%, 81%, se"]
This dropdown gives you the ability to rotate the icon. For example, you could use it to have an arrow point left, up, or down instead of right.
[/ui-callout-item]
[ui-callout-item title="Select" position="91%, 75%, se"]
Use the green **Select** button to lock in your icon of choice (listed in the text directly to the left). To choose a icon, simply select the checkbox in that icon's listing in the icon browser.
[/ui-callout-item]
![](icon_picker_1.png?classes=shadow,border)
[/ui-callout]

## Adding the Icon Picker to Your Site

The Icon Picker is a Gantry 5 input. If you want to add it to your theme or particle, you would do so by assigning the administrative input as `input.icon` in the associated YAML file.

Here is an example of the YAML code needed to add an **Icon Picker** field to a particle's settings which would then be made available to you in the particle.

```yaml
icon:
  type: input.icon
  label: Icon
  description: Select the icon you would like to use.
  default: fa fa-rocket
```

One great example of this field in action is in the **To Top** particle, which is part of Gantry 5's core particle set.

[ui-tabs position="top-left" active="0"]
[ui-tab title="Joomla"]

You can find the `totop.html.twig` and `totop.yaml` files located in `ROOT/media/gantry5/engines/nucleus/particles/`.

[/ui-tab]
[ui-tab title="WordPress"]

You can find the `totop.html.twig` and `totop.yaml` files located in `ROOT/wp-content/plugins/gantry5/engines/nucleus/particles/`.

[/ui-tab]
[ui-tab title="Grav"]

You can find the `totop.html.twig` and `totop.yaml` files located in `ROOT/user/plugins/gantry5/engines/nucleus/particles/`.

[/ui-tab]
[/ui-tabs]

Here, you can see exactly how the `input.icon` field is added to and utilized in the particle.


You can find more information about how to use YAML files in Gantry 5 [in our guide](../../advanced/particle-yaml-field-types).
