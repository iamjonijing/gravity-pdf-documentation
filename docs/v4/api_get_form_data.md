---
title: "get_form_data()"
sidebar_label: "get_form_data()"
description: ""
---

**Jump To Section**

* [Description](#description)
* [Version](#version)
* [Parameters](#parameters)
* [Return](#return)
* [Usage](#usage)
* [Source Code](#source-code)

### Description 

This API method will return [the $form_data array](https://gravitypdf.com/documentation/v5/developer-php-form-data-array/) for a particular entry. 

### Version 

This method was introduced in Gravity PDF 4.4.

### Parameters 

entry_id | integer | required
:    The Gravity Forms entry ID

### Return 

array | WP_Error
:    Returns the full `$form_data` array on success, or `WP_Error` on failure

### Usage 

```.language-php
/* Get the form data for the Entry #260 */
$entry = GPDFAPI::get_form_data( 260 );

if ( ! is_wp_error( $entry ) ) {
   /* We can use the $entry array here */
}
```

### Source Code 

This method is located in `api.php`.