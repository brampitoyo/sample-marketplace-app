# Locales and listing

## Add, remove, and set a default locale

* You must select one default locale; to do this, suffix the folder-name with `-default`; a Japanese default locale would have the folder name `ja-default`.
* To enable a locale, create a new `.md` file that has the locale code as a name (see Appendix for a list of valid locales); a German locale would be named `de.md`

## Editing locale

* You can modify these fields:
  1. Name
  2. Description
  3. Release notes (optional)
  4. Homepage
  5. Support homepage
  6. Support email
  7. Privacy policy
* Every field above, except for release notes, is mandatory for a default locale
* Any other locale `.md` must contain at least 1 field
* Any field that’s not filled will fallback to the content found under the default locale’s `.md`

## Our recommendation

* Update the `Release notes` for every new version
* Localize the `Description` to the language of every country you support

## Appendix: a list of valid locales

* bg - Bulgarian
* bn-bd - Bengali (Bangladesh)
* ca - Catalan
* cs - Czech
* da - Danish
* de - German
* el - Greek
* es - Spanish
* fr - French
* gd-ie - Gaelic (Ireland)
* hr - Croatian
* hu - Hungarian
* it - Italian
* ja - Japanese
* ko - Korean
* mk - Fyro Macedonia
* nb-no - Norwegian (Bokml)
* nl - Dutch
* pl - Polish
* pt-br - Portuguese (Brazil)
* ro - Romanian
* ru - Russian
* sk - Slovak
* sq - Albanian
* sr - Serbian (Cyrillic)
* sr-latn - Serbian (Latin)
* tr - Turkish
* zh-cn - Chinese (China)
* zh-tw - Chinese (Taiwan)