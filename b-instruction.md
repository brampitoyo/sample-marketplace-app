# Get Started

Place every file and folder on the `root` directory of your web app folder

# Manifest Fields

## activities

Firefox OS only, optional

Specifies a set of Web Activities that this app supports. Each property in this field is an activity. Activity names are free-form text, and each activity is represented by an object. Here is an example activities field with one activity named share:

```javascript
"activities": {
  "share": {
    "filters": {
      "type": [ "image/png", "image/gif" ]
    },
    "href": "foo.html",
    "disposition": "window",
    "returnValue": true
  }
}
```

## appcache_path

Optional

The absolute path to the application cache (AppCache) manifest. When an Open Web App is installed, the AppCache manifest will be fetched and parsed, and its static assets under the CACHE header will be cached.

```javascript
"appcache_path": "/cache.manifest"
```

## chrome

Optional

Adds a navigation interface at the bottom of the screen. This is a quick way to give some navigation controls to an app that doesn't provide its own back button.

This option should be a last resort. Consider adding a back button to your app interface to provide the best user experience.

```javascript
"chrome": { "navigation": true }
```

## csp

Optional

Specify a Content Security Policy for the app. This policy gets applied to all pages loaded in the app.

## default_locale

Required

A language tag (RFC 4646) that tells what language your manifest uses. Do not include the language tag you use here in the `locales` field. The Firefox Marketplace will use it to know what language your manifest is in, so it can use the correct `locale` values in translated fields.

## description

Required

A human-readable description of the app (maximum length is 1024 characters).

## developer

Required

Information about the developer of the app. It has these properties:

* `name` - The name of the developer.
* `url` - The URL of a site containing more information about the app's developer. This URL is typically rendered when the user clicks on the name of the app's developer while viewing details about an app inside the dashboard (or browser).


## fullscreen

Optional, Firefox OS only

Set this to `true` or `false` to indicate whether the runtime should launch the app in full-screen mode. Example:

```javascript
"fullscreen": "true"
```

## icons

## installs_allowed_from

## launch_path

## locales

## messages

## name

## orientation

## origin

## permissions

## precompile

## redirects

## type

## version