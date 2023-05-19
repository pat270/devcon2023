# Liferay Companion Workspace For:

## How to Implement Your Design System in LXC Using Clay (DevCon 2023)

This workspace contains two examples of implementing the [Carbon Design System](https://carbondesignsystem.com/) as a Liferay [Theme CSS Client Extension](https://learn.liferay.com/w/dxp/building-applications/client-extensions/front-end-client-extensions/tutorials/using-a-theme-css-client-extension).

- *carbon-v11-direct-css-copy*

	This is a direct copy of Carbon's css. It's quick and easy but it will only work with markup designed for Carbon. As a result none of Liferay's components will be restyled to look like Carbon.

- *carbon-gray-100-v11*

	This example is applying Carbon's design system to Clay by using [Clay's](https://clayui.com/) Sass API. This takes a bit more work, but it results in all of Liferay's OOTB components also being styled to match Carbon's design system. This let's you leverage more of Liferay's features and will likely save you time in the long run.

## How to Deploy

1. Update `liferay.workspace.home.dir=` in your `gradle.properties` file to point towards your Liferay bundle.
1. From the `client-extensions` directory run `blade gw deploy`.