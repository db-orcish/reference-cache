# Structures

The base level of the repository store contains a directory per stored publisher. The directory name will be a condensed version of the publisher name with the following constraints: Replace spaces with _, drop remaining non-alphanumeric characters, lower case. This will probably work poorly for non-english names and advice will needed.

## publisher_root.json

This document will be stored within the publisher directory as publisher_root.json

|Field|Type|Contents|Required|
|-|-|-|-|
|simplename|String|An ascii8 version of the Publisher Name|Y|
|fullname|String|A UTF8 version version of the Publisher Name|N|
|homepage|String|URL for the publisher|Y|
|contact|String|Point of Contact email address for questions|N|

## title_root.json

There will be one copy of this document per released content. It should be named with the product SKU identifier.

|Field|Type|Contents|Required|
|-|-|-|-|
|title|String|Title of the Product|Y|
|system|String|Game System supported, if applicible|N|
|purchaselinks|List of String| A list of URLs to purchase the title|N|
|writers|List of Strings|Names of writers as listed in the Colophon|N|
|editors|List of Strings|Names of editors as listed in the Colophon|N|
|summary|String|Summary of the Book|Y|
|tags|List of Strings|A list of Genre and Content Tags applicible to the title|N|
|attributions|List of String|A list of OGC contributions used with this title, even if not included in the shared text|N|
|contributions|List of content objects|A list of contributed content from this title|Y|
|language|String|The UTF Codepage for this copy of the title|Y|

### content_root.json

This file represents the bits of content the document provides for sharing.

|Field|Type|Contents|Required|
|-|-|-|-|
|system|String|Game System supported, if applicible|N|
|writers|List of Strings|Names of writers as listed in the Colophon|N|
|editors|List of Strings|Names of editors as listed in the Colophon|N|
|tags|List of Strings|A list of Genre and Content Tags |N|
|attributions|List of String|A list of OGC contributions used with this title, even if not included in the shared text|N|
|category|string|A name value for the type of contribution. See Utility Data.|N|
|summary|String|A short, markdown description of the contribution|Y|
|richtext|Markdown Text|The markdown text block for the contribution|Y|
|language|String|The UTF Codepage for this copy of the contribution|Y|

## utility_data.json

This is a container file for fixed lists to be used for selection prompts so they are spelled consistantly. The file shows some examples.

The values in the example document are purely examples.

|Field|Type|Contents|
|-|-|-|
|tags|List of Strings|Genre tags for applications|
|categories|List of Strings|Category descriptors for the type of contribution|
|systems|List of Strings|List of systems a contribution may apply to|