# Country

* Every app must have at least one country or country’s operator associated with it
* To add a new country, create a new blank `.country` file named after a country (see Appendix for a list of valid countries); an app that’s available globally would contain a `global.country` file

# Price

* Every app must have a price
* To add a new price, create a new blank `.price` file named after a tier (see Appendix for a list of valid price tiers); an app that costs $0.99 would contain a `tier4.price` file

# In-app payment and products

## In-app payment

Support for in-app payment is automatically disabled. To enable it:
* Create a blank filename called `in-app.enable`
* Create a new folder called `in-app-products`

# In-app products

* Once you enable in-app payment, create a new folder called `in-app-products`
* Inside this folder, create a folder for every in-app product you create; an in-app product called “Magical Unicorn” might have a folder that’s named `unicorn`, `magical-unicorn` or almost anything.
* Inside each in-app product, you must put a `.price` file with the appropriate tier

# Payment accounts

* If your app has a price, it must also have at least one payment account
* To add a new payment account, create a new folder called `payment-accounts`
* Inside this folder, create a new `.provider` file (this file will __not__ be blank) named after a payment account provider you signed up for (see Appendix for a list of valid payment providers); if your app is signed up for Bango, you would create a `bango.provider` file
* These `.provider` files are not blank. Inside each file, you must provide a "username" and "token" values

# Appendices

## List of valid price file names

* free.price
* tier0.price - $0.00 (use this tier if your app is only going to be made free _for a period of time_)

### Only supports carrier billing
* `tier1.price` - $0.10
* `tier2.price` - $0.25
* `tier3.price` - $0.50

### Supports credit cards and carrier billing
* `tier4.price` - $0.99
* `tier5.price` - $1.99
* `tier6.price` - $2.99
* `tier7.price` - $3.99
* `tier8.price` - $4.99
* `tier9.price` - $6.99
* `tier10.price` - $9.99
* `tier11.price` - $12.99
* `tier12.price` - $14.99
* `tier13.price` - $19.99
* `tier14.price` - $24.99
* `tier15.price` - $29.99

## List of valid country file names

Use the operator prefix to make your app exclusive to that operator.

* `global.country` (using this means enabling every country on the list)
* `germany.country`
  * `germany-tmobile.country`
* `hungary.country`
* `mexico.country`
  * `mexico-telefonica.country`
  * `mexico-amx.country`
* `poland.country`
* `spain.country`
  * `spain_telefonica.country`

## List of valid payment provider file names

### Bango
* `bango.provider`
* Register for an account at: http://bango.com/
* Information needed:
  * Username
  * Token

### Provider Name
* `providername.provider`
* Register for an account at: http://providername.com/
* Information needed:
  * Username
  * Token