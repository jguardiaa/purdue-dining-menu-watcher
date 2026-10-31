# Purdue Dining Menu Watcher

## Goal
Never miss a favorite food at the Purdue dining courts. This script checks every dining court's menu for the day and tells you which court is serving something on your favorites list, and at which meal.

## MVP scope
- Fetches today's menus from Purdue's public dining API
- Matches menu items against favorites.txt
- Prints the court and meal period for every match
- Saves a dated snapshot of the day's menus

## Future plans
- Email alerts when a favorite is found
- Automatic daily runs via cron
- Weekly stats on how often favorites appear
- Separate favorites per meal

## Tech stack
Bash, curl, jq, grep, cron. Favorites stored in a plain text file, menu snapshots saved as JSON.

## Data source
Purdue's public dining menus API (free, no key): https://api.hfs.purdue.edu/menus/v2/locations
