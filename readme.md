# jquery for lunet

This extension allows to easily integrate jquery in a lunet project.

## Usage

In the `config.sban` of your site, add the following command:

```
extend "jquery"
```

## Configuration

By default, this extension will try to download the latest version of the npm/jquery package and install it to the private `.lunet` directory.

It will be added to the default bundle.

The following variable can override the `jquery` module loaded. They have to be setup before using `extend "jquery"`:

- `default_bundle`: name of the default bundle to add jquery
- `jquery_provider`: name of the jquery provider (by default `npm`)
- `jquery_version`: jquery version to use (default is latest)
- `jquery_public`: true if jquery resource must be installed to the public directory _meta/resources/npm/jquery (default is false)
- `jquery_pre_release`: true if it allows to use a pre-release version (default is false)
