URL Field
======================

Specialized field for attaching internal cool links or external links in Symphony CMS.


## 1 About

This field depends on Entry URL field. Install it before continuing.

It allows the cool linking between Symphony entries so you will never have dead links any longer.


## 2 Installation

0. Install Entry URL field.
1. Upload the `url_field` folder in this archive to your Symphony `extensions` folder.
2. On `System -> Extensions` page install it by selecting the `Field: URL`, choose `Enable/Install` from the `With selected ...` menu, then click `Apply`.
3. The `URL` field will be available in the list when creating a Section.


## 3 Usage

1\_ Add an Entry URL field named `View on site` to a `Section A` (I assume you have a `Text box` with name = `Title`):

Set a slick value for `Anchor Label`: `Link of "{entry/title}"`<br />
Set a slick value for `Anchor URL`: `/entries/{entry/title/@handle}`

2\_ Create some entries in `Section A`.

3\_ Go to `Section B` and add URL Field to it. Select `View on site` from `Section A` in `Values` selectbox.

4\_ Create an entry in `Section B`. You can swtich between `Internal` and `External` links. Internal select will
be populated with all entries from `Section A`.

For External links, the value must be a valid URI.

If you don't select any sections in field settings, the field will accept only External links.
