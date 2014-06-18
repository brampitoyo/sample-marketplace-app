# Locales and listing

## Add, remove, and set a default locale

* To add a new locale, create a new blank `.locale` file that has the locale code as a name (see Appendix for a list of valid locales); an American English locale would be named `en-us.locale`
* You must set one locale as a default; to do this, give the file name a `-default` suffix; a Japanese default locale would have the file name `ja-default.locale`.

## Editing app listing inside each locale

* Inside each `.locale` file, you can add and modify these fields:
  * ## Name
  * ## Description
  * ## Release notes
  * ## Homepage
  * ## Support homepage
  * ## Support email
  * ## Privacy policy
* Your default locale file **must contain every one of the field above**, except for Release notes
* Any other locale file can contain any number of field
* Any field on any other locale that’s not filled will fallback to the content found under the default locale’s `.md`

## Our recommendation

* Update the `Release notes` for every new version
* Localize the `Description` to the language of every country you support

## Appendix: valid locale file names

* `bg.locale` - Bulgarian
* `bn-bd.locale` - Bengali (Bangladesh)
* `ca.locale` - Catalan
* `cs.locale` - Czech
* `da.locale` - Danish
* `de.locale` - German
* `el.locale` - Greek
* `es.locale` - Spanish
* `fr.locale` - French
* `gd-ie.locale` - Gaelic (Ireland)
* `hr.locale` - Croatian
* `hu.locale` - Hungarian
* `it.locale` - Italian
* `ja.locale` - Japanese
* `ko.locale` - Korean
* `mk.locale` - Fyro Macedonia
* `nb-no.locale` - Norwegian (Bokml)
* `nl.locale` - Dutch
* `pl.locale` - Polish
* `pt-br.locale` - Portuguese (Brazil)
* `ro.locale` - Romanian
* `ru.locale` - Russian
* `sk.locale` - Slovak
* `sq.locale` - Albanian
* `sr.locale` - Serbian (Cyrillic)
* `sr-latn.locale` - Serbian (Latin)
* `tr.locale` - Turkish
* `zh-cn.locale` - Chinese (China)
* `zh-tw.locale` - Chinese (Taiwan)