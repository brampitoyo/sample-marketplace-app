Welcome to the `sample-marketplace-app` repository!

# What

This repository is designed to show you two things:
* How the entire app management can be outsourced from a cumbersome graphical user interface to either:
  * One big `manifest.webapp` file, or
  * A few semantically meaningful files and folders
* How devhub can exist as a very lightweight publishing service on top of any repository

# Why

The problem we needed to solve was the fact that an app has a lot of elements, but a developer would rather not deal with these elements using an unfamiliar interface. So we thought: why not make the repository contain every app information that’s needed for submission?

We realize that:
* Virtually every app developer uses a text editor or an IDE
* Virtually every app developer uses some sort of a code repository
* Learning and getting used to a new graphical user interface is cumbersome

So we thought, why not use the code itself or a set of plaintext files and folders as an interface to submit an app to devhub?

The benefits are, we reckon, quite significant:
* App submission is integrated right into the developer’s workflow. We don’t say “Text editor is where you code, and devhub is where you submit and manage”. Every other marketplace in the world do this. Rather, we say “Do everything in code and plaintext, using your favourite text editor and code repository, locally or remotely. Submit with one button.”
* By integrating with a version control system, collaboration within teams and global community contribution becomes easy to manage
  * The localization team, or those interested to contribute in localization, can work on the `/locale` folder, or that section of the manifest
  * The finance department can work on the `/country-price-payment` folder, or those sections of the manifest
  * The design team, or those interested to contribute in design can work on the `screenshots-videos` folder, or that section of the manifest

# How

Two possible approaches:

1. Expand the manifest to include every possible information (see `manifest-full.webapp`). This includes the information that it doesn’t cover today, like categories, release notes, ratings, price, and availability.
  * Pros: One file to rule them all. Developer would only need to worry about one file.
  * Cons: Manifest becomes non-standard/non-spec.

2. Minimize the manifest (see `manifest-minimal.webapp` and the `/marketplace` folder). Every piece of information about an app has its own file.
  * Pros: The status of the whole app can be inferred just by looking at the file and folder structure.
  * Cons: Must manage many files.

# How to preview the work

## First approach

* Open `manifest-full.webapp` (we’re not using `manifest-minimal.webapp` in this approach)

## Second approach

* Open `manifest-minimal.webapp` (we’re not using `manifest-full.webapp` in this approach)
* Go to the `/marketplace` folder:
  * Look at the `README.md` file inside each folder for further instruction
  * Most files with custom prefixes – `.price`, `.country`, `.category`, etc. – are blank
  * But files with the `.locale` and `.provider` prefixes are not! They contain information needed, like payment account, app description, and so on