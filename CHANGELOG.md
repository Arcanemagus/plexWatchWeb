# 1.7.0-2 dev
* Change: more UI tweaks
* Add: Add sorting icons to users table header (@Arcanemagus)
* Fix: Fix sorting user list by time (@Arcanemagus)
* Add: Properly handle missing thumbs (@Arcanemagus)
* Fix: Fix functions 5.3.3 compatibility (@Arcanemagus)
* Change: User history - stream info modal header updates
* Add: Display errors for AJAX requests (@Arcanemagus)
* Fix: Fix the info modal
* Change: Modals / Stats minor UI tweaks
* Fix: Don't grab session data for library stats (@Arcanemagus)
* Change: Minor table UI tweaks
* New: UI Changes
* Change: Minor cleanup of charts (@Arcanemagus)
* Change: PHP 5.3.3 compatibility (@Arcanemagus)
* Fix: Security fixes (@Arcanemagus)
* Add: Show all IP addresses in user page (@Arcanemagus)
* Change: Upgrade Font-Awesome to v4.3

# 1.7.0-1 dev
* Change: Switch to using PDO for database access (@Arcanemagus)
* Change: Adjust status variable in `getPMSUrl` (@timrettop)
* Change: Error handling update (@Arcanemagus)
* Add: Plex HTTPS support (@Arcanemagus)
* Fix: Fix Season thumbnails (@Arcanemagus)
* Fix: Fix issue where times are displayed incorrectly in certain areas if PHP's
time zone is different than the system's. (@ghost)

# 1.7.0 dev
* New: global: Icon support for KODI, Sony PlayStation, and Opera clients
* Change: Code cleanup (@Arcanemagus)

# 1.6.2 dev
* Fix: get-library-stats.php: Fix for user count == 0 (@rbowden91)
* Change: stats.php: Extended monthly plays chart to one full year, including
year of month

# 1.6.1 dev
* Fix: info.php: `$row['date']` definition for line 815 (@ljm42)
* Fix: info.php / user.php: Fallback to Grandparent poster if parent poster
isn't available. If all else fails, drop back to image placeholder. (@Keelan)
* Fix: Patch to address the `img.php` vulnerability. (@drzoidberg33)
* Fix: Store plex.tv password base64 encoded (in case someone is looking over
your shoulder) (@drzoidberg33)
* Fix: user.php: Samsung and Xbox platform icons were not appearing.
* Removed: settings.php: "PMS Secure Web Port" and "Use HTTPS" are no longer
usable options with PMS so they were removed.
* Change: settings.php: Plex Authentication title and description were reworded
so users better understand the need to enter this data if using "Plex Home"

# 1.6.0 dev
* Add: global: Server side processing for history tables. (@drzoidberg33)
(note: `info.php` table code needs revised)
* Add: global: Icon support for Xbox consoles.
* Fix: info.php, recently_added.php: Added input validations (@m33x)
* Fix: settings.php, user.php: XSS vulnerabilities (@m33x)

# 1.5.4.2 master
* Fix: global: API call contained an invalid parameter
(merged pull request #62 from @ljunkie)
* Fix: current activity: Music thumbs would not always display

# 1.5.4.1 master
* Fix: current activity: Minor CSS change to fix offset username in current
activity instances.
* Add: global: Additional platform images for future use.

# 1.5.4 master
* Fix: global: PMS owners with no Gravatar account would display broken user
avatar images.
* Change: global: Minor CSS and layout tweaks
* Add: global: Additional `php5-sqlite` checks to alert users if they are missing
the requirement

# 1.5.3 master
* Add: index.php: Current Activity now supports music tracks
* Add: index.php: Current Activity now reports if a user is "buffering"
* Change: index.php: Current Activity CSS modifications
* Change: global: Date columns in all tables are no longer restricted to `/` delimiters
* Add: settings.php: Date/Time options modal
* Fix: global: Broken platform image link would appear if client source was
reported as Plex/Web (Unknown Browser)

# 1.5.2 master
* Fix: settings.php: Form portion of settings page was inaccessible if plexWatch
database location value was set incorrectly
* Fix: global: Date columns were still not sorting properly in all data tables
if a date format other than `m/d/y` was used

# 1.5.1 master
* Fix: global: Date columns were not sorting properly in all data tables

# 1.5.0 master
* Change: Version bump to master
* Change: global: Updated welcome logo to match new Plex logo.

# 1.5.0.14.2 dev
* Fix: global: Stream video details width and height were being displayed under
audio column when stream was direct play type
* Change: global: Updated logo to match new Plex logo.

# 1.5.0.14.1 dev
* Fix: user.php: Platform stat total plays were not matching all time total
plays when grouping was enabled

# 1.5.0.14 dev
* Change: global: Separated stats from history logs and created a new page for
them
* Add: global: Stream info column in history tables which links to a modal
containing stream and source details
* Fix: index.php: Recently added items would sometimes wrap to a second row
depending on width of browser

# 1.5.0.13 dev
* Fix: info.php: Season episode thumbs and top watched episode thumbs would not
appear if using internal LAN IP address for PMS and Plex authentication was
disabled.

# 1.5.0.12 dev
* Fix: global: Minor CSS adjustments for IE

# 1.5.0.11.2 dev
* Fix: global: Additional Samsung platform icon support issues

# 1.5.0.11.1 dev
* Fix: global: Samsung platform icon support (@rcork)

# 1.5.0.11 dev
* Add: global: Samsung platform icon support

# 1.5.0.10 dev
* Remove: users.php: Table column sorting is locked to alphabetically by user
until a fix is available for "last seen" column
* Change: user.php: Minor CSS tweaks to stats
* Change: current_activity.php: Minor tweaks to direct stream audio codec names
* Fix: global: Apple TV platform icon did not appear when client device was
PlexConnect

# 1.5.0.9 dev
* Fix: global: Duration times were incorrect for user and media history tables

# 1.5.0.8 dev
* Fix: global: Table date sorting by newest date would not sort properly when
the year was different (This fix has a current limitation that requires `/` as
the delimiter between day, month and year)

# 1.5.0.7 dev
* Fix: user.php: Incorrect platform image could appear when user grouping was
enabled
* Change: user.php: Public IP address platform to "Platform (Last Seen)" and
include Chromecast as possible platform

# 1.5.0.6 dev
* Add: global: Differentiate Chromecast from Plex/Web (Chrome) platforms
(current plexWatch DB limitation does not allow user platform stats seperation)
* Fix: global: undefined `fileContents` variable on initial use

# 1.5.0.5 dev
* Fix: global: Table date column sorting fix from 1.5.0.4 did not work.
Defaulting formatting with year first for now until there is a better fix

# 1.5.0.4 dev
* Fix: global: Table date column sorting by newest date would not sort properly
when the year was different
* Change: settings.php: "myPlex" has been renamed "Plex Authentication" to
maintain consistency with Plex.tv's removal of the myPlex name
* Fix: history.php: Monthly plays chart would not display next month in a new
year properly
* Change: current_activity.php: Design and CSS adjustments
* Change: global: CSS and image changes to maintain consistency with upcoming
Plex/Web v2.0
* Fix: history.php: Left chart padding was cutting off display values above 999
* Add: global: User definable date & time formats from `settings.php`
* Change: global: Minor layout changes / added page headers
* Remove: info.php: Movie details - commented out writers list to help maintain
a more consistent height

# 1.5.0.3 dev
* Add: PHP5-JSON to readme requirements. Check for JSON support in settings
welcome modal
* Change: Hard coded plexWatch/Web version number into `settings.php` so users
don't have to re-save their configuration after every update in order to see
the proper version number
* Change: history.php: Chart widths are now dynamically set for better tablet
and mobile viewing

# 1.5.0.2 dev
* Add: user.php: Separated IP address information from user history by including
a new tab
* Change: users.php: Modified user list to use table view which includes more
details about each user
* Add: history.php: Max hourly plays (@ljunkie)
* Fix: index.php: Fix hardcoded library section (@ljunkie)

# 1.5.0.1 dev
* Remove: index.php: Plex status which was really just a placeholder
* Add: index.php: Plex Media Server stat section counts (Movies, TV shows, Users)
* Change: global: Minor font size changes
* Change: charts.php: Top 10 episodes now use show poster rather than season
poster

# 1.4.1 master
* Fix: global: Attempt to correct error related to `simplexml_load_file`
(@billimek / @sunnyd71)

# 1.4.0 master
* Change: Version bump to master

# 1.4.0.11 dev
* Add: myplex.php: XML parse error checking when trying to authenticate with
myPlex
* Add: settings.php: PHP-cURL error checking when trying to authenticate with
myPlex

# 1.4.0.10 dev
* Change: info.php: Icons for table heading
* Change: global: Main menu icon for users
* Fix: global: Gravatar image for a 404 response would display no image
* Change: Version numbering scheme adjustment. It should now follow this scheme
(major.minor.maintenance.development) (branch: master, dev, etc)
* Add: user.php: Included a few more platform checks from DB platform if XML
platform is empty (Apple TV)
* Change: user.php: Changed geo location providers since ipinfo.io seems
unstable
* Add: user.php: Initial platform play count stats
* Add: user.php: Platform column for user public IP address history
* Add: user.php: Check for region name result for public IPs. Display "n/a" and
remove link if result is empty
* Add: user.php: Play count column for user public IP address history
* Fix: user.php: IP addresses were being filtered incorrectly
* Change: index.php: *BETA, NEEDS MORE TESTING* Recently added items now display
a dynamic amount based on row width. This used to be a fix amount (10).
(@ljunkie)
* Add: global: Friendly name+platform support (@ljunkie)
* Change: settings.php: Now includes a navigation list
* Add: history.php: Hourly, daily and monthly play count charts
* Change: global: Modified the way plexWatch/Web retrieves image from PMS to
hide myPlex authentication token	(thanks to @ljunkie, @ryanc, @dashbad & *=Matt=*
for their ideas and examples)
* Add: myPlex authentication support for accessing plexWatch/Web from remote
networks
* Add: Introduction welcome screen modal with requirements quick test and
briefing
* Change: charts.php: Minor CSS adjustments to help with alignment issues
* Change: Main menu change from text and icons to just icons (font-awesome) with
tooltip on hover (same as Plex/Web). This allows mobile header to maintain the
standard height dimension
* Add: user.php: User IP address history with geo tag location, Google maps link
and ISP information
* Add: Grouping support which is user selectable for history, user history and
charts
* Add: settings.php: New page with full support for configuring plexWatch/Web.
`config.php` is written dynamically by settings.php and was relocated to
`/config/config.php`. This file no longer needs to be edited by the user.

# 1.3.0
* Fix: info.php: If content was deleted from PMS and watching history links to
`info.php` with this information, an error to the connection was displayed. A
message now lets the user know "This media is no longer available in the Plex
Media Server database"
* Add: info.php: Season episode list if displaying season information
* Fix: info.php: If `genres` variable is not available it throws an error
* Fix: info.php: If `actors` variable is not available it throws an error
* Fix: index.php: Recently added season & episode information was incorrect.
PMS does auto grouping of episodes for a season so only the season number is
available when using this method.
* Fix: current_activity.php: Movie stream activity would not appear
* Fix: More divide by zero fixes (rcork)
* Add: global: Link logo to main page (rcork)
* Change: index.php: Current activity stream and codec details now better mimic
the terminology PMS and Plex/Web use (thanks rcork)
* Fix: history.php: Divide by zero errors (thanks rcork)
* Fix: info.php: Poster image sizing issue with Safari on Mac (thanks rcork)
* Add: global: Default poster image for results that do not have an associated
poster image
* Fix: index.php/user.php: Recently added / recently watched poster images would
not appear if user moved or deleted item from PMS database
* Add: config.php: Plex Media Server HTTP/HTTPS support including independent
port numbers
* Add: index.php: Current activity now supports "clips" from your myPlex queue
* Fix: info.php: If `writers` variable is not available it throws an error
* Add: global: Check if PMS server and plexWatch database are accessible. print
error output to user if they are not
* Add: config.php: Plex Media Server port variable added for users using
non-standard PMS ports

# 1.2.0
* Fix: index.php: First recently added result was getting cut off on left side,
changed episode image to season thumb
* Fix: global: Updated images in Plex/Web would not appear in plexWatchWeb
* Change: user.php: General usage stats changed from minutes to days, hours,
minutes
* Add: user.php: User profile tab with avatar image, general usage stats and
recently watched list
* Change: user.php: History table has been moved to a separate tab to make room
for profile and chart tabs
* Add: Tables: In-progress streams are now reported in the date column as
"Currently watching..."
* Change: Table row and cell colors altered to allow for better identity of
important elements and links
* Fix: tables: "Stopped" time would show and incorrect value if row element was
empty due to an in-progress stream
* Fix: Inconsistent time zones between `history.php`, `user.php` and `info.php`
* Change: Time zones are now automatically checked and set to webserver's
default time zone
* Wiki: Information for XAMPP users	about setting time zone and password
protection

# 1.1.0
* Initial public release

# 1.0.0
* Initial internal version
