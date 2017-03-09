# EVE Trade Finder v2.15

## About
Implements the EVE Crest API to find:

* the best trades between the major trade hubs.
* the best margins inside your own station

Select which of the 5 trade hubs you are docked in:

* Amarr
* Dodixie
* Rens
* Hek
* Jita

It will return a lazy-loaded table of trades you can make at other trade hubs. Allows table sorting on any of the fields to see what items are selling at your hub for a low price and can be sold at another hub for a higher price.

### V2.15 Implemented Profit filtering
* Ability to filter profits to show only rows where ISK is greater than N on route trades
* Ability to filter ROI to show only rows where ROI % is greater than M on route trades
* Ability to filter Buy Cost to show only rows where Cost is less than O on route trades
* Fixed a bug with station trading where it shows the wrong station's information
* Updated UI to appear a little more clean

### V2.14 Implemented Multi-sorting tables
* Now by shift + clicking a header row you are able to sort on additional properties.
* Added a Release Notes page

### V2.13 Updated UI
* Easier to select intro button
* Added description of each selector

### V2.12 Minor tweaks
* Removed minified files as they are minified automatically on the server
* Updated wording and about pages to be more concise
* Added designed and developed by fields

### V2.11 Emergency Hotfix
* Route changed to https://crest-tq.eveonline.com/market/{ID}/orders/sell/?type=https://crest-tq.eveonline.com**/INVENTORY**/types/{TYPE}/

### V2.1 Filter Patch
* Addition of filtering of columns with preset columns to make tables a little more mobile responsive on small width screens.

### "Margin Trading" Update v2.0
* Added functionality for margin trading within a station

### The "App-in-an-App" Update v1.2
* Allows user to view all active orders - buy and sell for a specific item on shift + click
* Only ctrl + click selects all now
* Updates algorithm to return better profit results
* Lazy load the item IDs from EVE's API and shuffles them
* Added YUI Compressor and Scripts to automatically created and deposit minimized code to proper directories
* Improved Trade info layout to use bootstrap columns
* Removed unused log statements
* Trade info sets to fixed decimals to improve sorting
* Made error messages more hospitable and do not show up multiple times
* Updated endpoint to not receive CORS as frequently

## The "Increased Functionality" Update v1.1
* Minified CSS and Javascript to improve performance
* Addition of multiple orders (up to top 3 for an item)
* Buy/Sell quantity columns added with highlighted recommendation
* Highlighting capabilities improved. Highlight one or multiple.
* Right-click to update the item.
* Updated UI to include start location, and end location(s) to reduce calls to hubs you are not intending to go
* Updated UI to better fit on smaller screens
* Stop button updates and provides feedback
* Moved init.js to the top through an on document ready function
* Added an unreachable notification if EVE's servers are down
* Moved to AJAX call structure rather than simple Jquery GET
* Updated number returned to between 1-10
* Moved all minified JS to one file
* Improved breakpoints for text and buttons on smaller screens
* Updated color scheme
* Moved CSS away from JS into CSS
* Updated footer
* Added stop functionality to stop loading if the user does not wish to continue
* If same destination and start point occurs it throws an error
* Unhighlights destination if start location is selected
* Buy Cost was not being calculated properly
* Update no longer returns just the top trade for all 3 slots
* Update graphic now just changes opacity. Less intrusive.
* Update now removes any lingering updates if not updated in 25 seconds.
* Algorithm was not always returning the most profitable runs  if runs > 3
* CTRL or SHIFT available to select all of an item type


Copyright © 2016-2017 Alexander Whipp
