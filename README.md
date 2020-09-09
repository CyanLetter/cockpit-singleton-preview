# Cockpit Singleton Preview

A collection of files to add / replace in a Cockpit CMS install, to enable content preview in Singletons. The majority of these changes are copied directly from the preview code for Collections.

**Tested with Cockpit version 0.10.0 only** - May not be a drop-in replacement for newer versions.

## Usage

As always, back up your files before overwriting anything.

These files replicate the folder structure of a Cockpit installation. You can either merge this repository with your existing cockpit installation, or manually add the files from this repository into your `modules/Singletons` folder.

- Drag the `assets` folder from the repository into the `modules/Singletons` folder of your Cockpit installation.
- Drag the two files in the `views` folder of this repository into the `modules/Singletons/views` folder of your Cockpit installation. Overwrite the files which were there previously.

That's it. You should be able to enable and use content preview in Singletons, the same way you can with Collections.

You can diff the files in this repository with the original versions in the initial commit to see what exactly changed.

## Why

While using Cockpit for a client project, I had built out the content assuming "singleton" was meant to be the same thing as "singles" or "single pages" in other content management systems. For various reasons, it was not feasible to re-create the single pages as collections, and thus this fix was developed instead.

See [this forum thread](https://discourse.getcockpit.com/t/preview-for-singletons/1247) and [this one](https://discourse.getcockpit.com/t/singletons-vs-regions/316) for discussion on what singletons are intended to be used for, and why the preview feature is not available for them by default.
