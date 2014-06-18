Go to the `/marketplace` directory in order to access app information required for submission to Firefox Marketplace.

The problem we need to solve is:
* An app has a lot of elements: from description to ratings. A valid app must have all these elements.
* The aim of putting information on the repository is the fact that we are integrating the submission process into the developer’s workflow. There’s no website to go to and no form to fill. Put simply, do everything that’s submission-related on the repository itself.
* We have three possible approaches:
  * Expand the manifest to include every possible information. This includes the information that it doesn’t cover today, like categories, release notes, ratings, price, and availability
    * Pros: One file to rule them all. Developer would only need to worry about one file
    * Cons: Manifest becomes non-standard/non-spec
  * Minimize the manifest, put all the other app information in its own files (a file to specify screenshots, another file to specify each locale, another file to specify category, etc.)
    * Pros: A pretty clean division of information. The manifest won’t need to contain everything and be overwhelming to manage.
    * Cons: There will inevitably be more files to manage. But the good thing is, it works great in team. I can tell my localization team to only touch the `/locale` folder. I can tell my 
