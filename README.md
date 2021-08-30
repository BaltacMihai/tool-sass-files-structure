# Sass File Structure

This is the structure of the sass files that I use and recommend. It is very important to have the same folder structure in all your projects, so it is easier for you to navigate and modify the project.
I don't use all the folders everywhere (some projects may not have themes, etc.).
I also recommend using the BEM convention to name classes.

# How is it used?

Only the main.scss file is compiled, it imports the other files.

Example:

```sass
@import "base/module";
```

Where the ___base___ is the folder and ___module___ is the imported module (where in turn it will import sass files from that specific folder).

!! pentru a nu se complia fisierele .scss, punem un " _ ", astfel avem "\_variable.scss"

## Base
contains global styles, such as resets, typography, colors, etc.

Example:

```sass
@import "colors";
@import "typography";
```

## Components

contains each self-contained component in its own .scss partial

Example:

```sass
@import "card";
```

## Layout
contains styling for larger layout components


Example:

```sass
@import "nav";
@import "header";
@import "container";
@import "footer";
```

## Pages
contains page-specific styling, if necessary


Example:

```sass
@import "html";
@import "homepage";
@import "about";
```

## Themes
contains styling for different themes


Example:

```sass
@import "default_theme";
@import "white_theme";
@import "dark_theme";
```

## Utills
//contains global mixins, functions, helper selectors, etc.



Example:

```sass
@import "responsive";
@import "animations";
```


















