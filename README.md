# Kavita Reading Log
Generates a static Kavita reading log one-page site

## Simple Setup
* Place kavita-reading-log.py and index.html in the same folder (may modify and move kavita-reading-log.py up a level and change json write location if you wish)
* Edit the settings at the top of kavita-reading-log.py (ODPS url, and any exclusions / label groups)
* Run kavita-reading-log.py to generate reading-history.json
* index.html uses this file, to serve your reading log.

## Notes
* If running locally, fetch is blocked by most browsers. You may have to spin a quick web server (such as `python -m http.server 8000`)
* This makes a LOT of API calls. Run it locally to Kavita, wherever it runs, for best results
* I suggest putting the kavita-reading-log.py on a cron for every x hours / days.
* Be sure to filter anything you want using the provided settings.

## Points to Improve (may or may not happen)
* Static order of tabs (goes most recent to least)
* Sortable order of items (goes most recent to least)
* Metadata (if desired)
* Better automatic filtering (tag, etc)
