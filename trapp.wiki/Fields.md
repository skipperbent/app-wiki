# Overview
In this section you can see what fields are supported and read more about them.

|Name|Type|Required|
|---|---|---|
|[locale](#locale)|string|true|
|[translate_into](#translate_into)|string|true|
|[deadline](#deadline)|datetime|true|
|[fields](#fields)|object|true|
|[comment](#comment)|string|false|
|[state](#state)|string|false|

-

### <a name="locale"></a> locale
Locale code for the content.

###### Type
string

###### Example
da_dk
en\_gb

###### Requred
True

-

### <a name="translate_into"></a> translate_into
Locale code that you want the content to be translated to

###### Type
string

###### Example
da_dk 
en\_gb

###### Requred
True

-

### <a name="deadline"></a> deadline
Datetime that specifies the last due date for the translation.

###### Type
datetime (WC3)

###### Example
2005-08-15T15:52:01+00:00

###### Requred
True

-

### <a name="fields"></a> fields
Fields that you want translated.

The object contains 3 required fields: 

- **label**: the name of the item. This value will be the one displayed for the translators.
- **value**: the text that you want translated - should be in the same language as the locale field provided.
- **displayformat**: wysiwyg for WYSIWYG editor, otherwise this can be ignored.

Any additional parameters provided will also be stored and will be displayed in the API.

###### Type
object

###### Example
{ "label": "Test", "value": "My text in the original language", "displayFormat": "wysiwyg" }

###### Requred
True

-

### <a name="comment"></a> comment
Comment to the translator.

###### Type
string

###### Example
Please remember to translate the image-text.

###### Requred
False

-

### <a name="state"></a> state
ID for the state which the content is currently in.

###### Type
string

###### Example
asda28391238asdasdasd

###### Requred
False