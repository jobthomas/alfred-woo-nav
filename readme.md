## Credits 

* Inspired by WPCOM workflow by Chris
* Workflow icon: https://www.iconfinder.com/icons/211784/navigate_icon

## WooCommerce Navigation Workflow

### What's this?

This Alfred workflow to guide user to navigate WooCommerce configuration option by pasting the path to the front most app on your mac.


### Is it useful to me?

Only if your work includes sending instructions on accessing various WooCommerce features and configuration options :) 

## Setup

1. Download `WooCommerce Navigation.alfredworkflow`
2. Install the workflow on your device
3. Search for navigation paths by `wn YOUR_QUERY`


## Usage

### `wn YOUR_QUERY`

* By default, the keyword is set to `wn` for stock configuration options
* Eg: If you want to search for the configuration path for `Hold Stock`, launch alfred and type `wn hold stock`:
    ![https://d.pr/i/CW0r3H+](https://d.pr/i/CW0r3H+)
* Output would be: `WP Admin > WooCommerce > Settings > Products > Inventory > Hold stock (minutes) > Define - Hold Stock in minutes`

### `wnb YOUR_QUERY`

* Same as `wn`. Only difference is that the output would be bold (markdown)
* Eg: The same query above, using `wnb` results in: `**WP Admin > WooCommerce > Settings > Products > Inventory > Hold stock (minutes) > Define - Hold Stock in minutes**`

### `wns YOUR_QUERY`

* Same as `wn`. Output is bold (HTML).
* Eg: The same query above, using `wns` results in: `<strong>WP Admin > WooCommerce > Settings > Products > Inventory > Hold stock (minutes) > Define - Hold Stock in minutes**</strong>`

### `wnca NAME|PATH`

* This would add a new, custom navigation path to a separate db table
* Make sure that the custom path does not have the same name as any of the existing stock names. This is because the workflow only searches the custom database if there are no results found for your query in stock database
* Custom path is saved in a different table so that if there's an update to this workflow in the future, your custom paths are not lost

### `wncr NAME` or `wncr PATH`

* Removes the custom name|path combination that you've added
* **This is irreversible** as there's no backup of custom table anywhere outside of your device
* Please also note that **there is no warning** prior to removing a custom item

