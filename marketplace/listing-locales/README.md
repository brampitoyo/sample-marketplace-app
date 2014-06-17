# Locales and listing

## Add, remove, and set a default locale

* To add a new locale, create a new `.md` file that has the locale code as a name (see Appendix for a list of valid locales); an American English locale would be named `en-us.md`
* You must set one locale as a default; to do this, give the file name a `-default` suffix; a Japanese default locale would have the file name `ja-default.md`.

## Editing app listing inside each locale

* Inside each `.md` file, you can add and modify these fields:
  * ## Name
  * ## Description
  * ## Release notes
  * ## Homepage
  * ## Support homepage
  * ## Support email
  * ## Privacy policy
* Your default locale `.md` **must contain every one of the field above**, except for Release notes
* Any other locale `.md` can contain any number of field
* Any field on any other locale that’s not filled will fallback to the content found under the default locale’s `.md`

## Our recommendation

* Update the `Release notes` for every new version
* Localize the `Description` to the language of every country you support

## Appendix: valid locales

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