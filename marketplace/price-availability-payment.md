# Price

"tier4"

# Availability

"global"

# In-app payment

"enable"

# In-app product

* "50 Gems": "tier1"
* "Extra Lives": "tier2"
* "Magical Unicorn": "tier3"

# Payment information

* "bango"
  * Username: "john.doe"
  * Token: "ot9vob7char5ap3hyt6dov1wal4caic8i4dru3ok3cac2cat4e"
* "providername"
  * Username: "john.doe"
  * Token: "rark7yez8ju3wyk0jak3gav3hec6oij4riemth1ag7he7of6un"

# Appendices

## List of valid price values

* free
* tier0: $0.00 (use this tier if your app is only going to be made free _for a period of time_)

### Only supports carrier billing
* tier1: $0.10
* tier2: $0.25
* tier3: $0.50

### Supports credit cards and carrier billing
* tier4: $0.99
* tier5: $1.99
* tier6: $2.99
* tier7: $3.99
* tier8: $4.99
* tier9: $6.99
* tier10: $9.99
* tier11: $12.99
* tier12: $14.99
* tier13: $19.99
* tier14: $24.99
* tier15: $29.99

## List of valid availability values

Use the operator prefix if you’d like to make your app exclusive to that operator.

* global (using this means enabling every country on the list)
* germany
  * germany_t-mobile
* hungary
* mexico
  * mexico_telefonica
  * mexico_amx
* poland
* spain
  * spain_telefonica

## List of valid payment account values

See a diagram of (which payment provider supports which region)[]

### Bango
* Code: "bango"
* Register for an account at: http://bango.com/
* Information needed:
  * Username
  * Token

### Provider Name
* Code: "providername"
* Register for an account at: http://providername.com/
* Information needed:
  * Username
  * Token