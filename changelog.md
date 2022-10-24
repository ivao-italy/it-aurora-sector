# Changelog Staff Beta
## [1.2.22.32] - 2022-02-19
### Added
- Invalid message version.
- Press return key to connect when entering credentials/callsign
- Audio compressor to microphone input
- Visual feedback to disabled ATIS window button
- Live log view (right click on red beta label)
- Overhaul windows controls (Maximize, fullscreen, minimize)
- Minimize to tray
- Select windows to show when in tray mode
- Double click on titlebar to maximize
- Alt + Up Arrow to maximize
- World Servers to network and teamspeak server list

### Changed
- Saving and loading of the profile with encrypted credentials
- Better tooltips
- Logging system to store up to 10 files
- Auto select worldserver voice TS server when selecting worldserver network server

### Fixed
- Fix malformed profile.ini file
- Metar/atis/clock labels disappearing out of pvd bounds
- QDM/STCA track offset by mag deviation
- Speed unit conversion
- Overlapping traffic label (last selected traffic stays on top)
- FSD ATIS protocol bug
- METAR not showing in ATIS window (allow sector to fully load)
- Inset preferences saving
- Max limit with zoom range
- Zoom out max limit
- Names column disappearing from inset transfer list
- Failure to start if profile.ini does not exist
- Fix hang on close when settings was opened
- Connect menu position
- Duplicate keyboard shortcuts
- Inset context menu not showing
- Icons and tables size on high DPI displays and 4K monitors
- Context menu positioning (constraint to work area)

## [1.2.23.0] - 2022-04-13
### Added
- Message for forced/lost connection
- Add resizing to top bar
- Super heavy wake turbolence colorscheme support
- Map circular scroll
- Sector loading info on pvd
- Allow manual update
- World Server in Beta
- Staff version alert in title bar
- CTD logging
- CPDLC message filter by response type
- Connection lost message
- Add wheel scroll to FPL route, equipment and remarks fields
- Add wheel scroll to METAR field in traffic window
- Progress bar to update unzip process
- Drag info message window
- Info message window queue system
- Show changelog on startup after update
- Sector ICAO GEO Files explained in Sector
- Append "_WS" to intercom callsign if connecting to World Server
- Deletion and warning for presence of desktop.ini and update.ini in sector file update
- Do not extract hidden, readonly, archived or system files from sector file update
- Stack trace dump on sector load error
- Metric conversion to ATIS TA and TL
- Show "please wait message" when changing voice server too frequently
- SID/STAR <br> function
- Changed structure on CA / STCA / DUPE
- Add monitor traffic refresh to investigate interpolated track
- Add sector error in Logs\SectorError.log
- Sector log live monitor in log window
- Sector loading stats to debug log
- Current traffic gate on #TRPOS 3rd party packet
- 3rd party auto start
- Responsive buttons in airport window
- Server list cache in case of unreachable API
- Invert MVA and VFR buttons in airport window
- Traffic QDM can turn 360 degrees
- Auto update QDM manager data while window is open
- Scroll bar to changelog window
- Send text button in traffic manager
- Hand cursor to SEND and PM buttons in traffic manager
- Show timer while waiting for update on close

### Changed
- Major backend refactor
- Refactor thread interlock
- Set dct and time on route after labeling
- Overfly data cleared when added
- Pretty format control session recordings
- Improved airport labels performace when set as Controlled
- Check for updates after login
- Improved main radar performance when DMS info line activated
- Disabling DMS line improves framerate
- World Server address
- Refactor sector loading
- Read sector backend
- Sector file extraction in temp folder
- Sector painting optimizations
- Hoppie CPDLC messages format
- Default CPDLC messages
- Zoom smoothness
- Improved tfl drawing performance when zoomed in
- Smaller font on changelog window
- Bigger changelog window with syntax highlight
- Enable copy of readonly files
- Increased extrapolated track threshold
- Moved QDM data further away from cursor
- Send pm button in traffic manager now opens PM in comm box

### Fixed
- Column width on high dpi
- Column width in Airport screen
- Lines below comboboxes when small ui font or high dpi
- Intercom mouse wheel interaction
- Fix 4k screen border artifact at minimum zoom
- Fix overlapping controls on title bar
- Limit window max size to current size of monitor
- Fix save/load DEFA areas
- Nav aids label position
- Align to center arrows on traffic manager
- Trainer status check
- Names on ATC/Traffic
- Powershell failure preventing start
- Inset not showing ground traffic
- Speedvector position
- Fix position update after sector change
- Labels moving in inset when zoomed
- Auto active runways
- Traffic visibility filter inset
- Label lines with std SSR
- SID STAR info
- Hang when labeling SID/STAR
- TEXT label spurious showing
- Special areas internal handling
- QDM turn calculation
- Notams in inset
- Airport active runway bug
- Inset closest airports
- Comm box context menu position when not on main screen
- Hang when opening ATC window after traffic transfer
- Clearance context menu focus on inset
- Spurious "0" on traffic (halo related)
- Airport window, "show controlled only" wrong behavior
- Auto update sector file
- Vera QDM
- Multi QDM Removing
- QDM Manager data
- QDM Turn
- Airport filter
- INSET label symbols.
- Match TeamSpeak server to network server
- Cannot delete sector if not existing
- Server message popup when server refuses connection
- Double click required to expand inset if was opened in collapsed state
- Scroll in changelog window
- CPDLC window not expanding if saved as when collapsed
- CA / STCA / DUPE state not mirrored to both traffics
- GroundTexture Filter with Shift + GEO
- Inset causing CTD on 32 bit
- CA alert sound
- MVA labels not showing
- Improved 3rd party stability
- Cannot type in comm box
- Fix hang if closing while connected
- Fix sector stats logging STAR and SID count
- SID STARS labels position
- 3rd parties zoom and select command
- Profile CTRL/RW/VFR/MVA filters loading
- Missing hints in airport and atc window
- Single and multi QDM visual glich
- Test fix interpolated track
- Fix scrolling transfer list in PVD
- Traffic QDM selectable area
- Route data SID, STAR and enroute
- Autosize Draw Perf button on debug window
- Text fix access violation when assuming traffic
- Rectangle showing under route time
- Floating SEND button in traffic manager

### Removed
- Removed bold from free text and bay inputs
- Sector stats and autoscroll buttons from debug window

## [1.2.24.1] - 2022-05-22
### Added
- Allow running only one instance of Aurora
- New login UI (frontend only)
- New SSO login system
- Logout button
- Login fields validation
- Shadow to windows
- Resize on left border of main window
- User account window

### Fixed
- Rectangle showing under route time
- Floating  SEND button in traffic manager
- Clear sector files and directories attributes on unzip (system, hidden, archive, readonly)
- Main window disapparing if double clicking maximize/fulscreen
- Fix taskbar icon not showing after login splash screen
- Fix stipple line for dct on route
- Name characters encoding on login welcome message
- Trigger autoupdate on startup
- Login and connect window on scaled screens
- Trainer/examiner role check
- Settings button disappearing
- Trainer/examiner role check
- CTD on startup if profile.ini is empty
- IVAN and TS2 server selection
- Vector line on PSR
- IVAN password login
- ATIS window size
- QDM not moving from traffic to traffic
- Null division prevend user login and result in CTD
- Memory leak on SSO HTTPS requests
- SSO token refresh interval
- Fix right click menu DEFA TXT control alignment
- Crash when closing while sector is loading
- NaN aicraft track direction
- Hanging voice when using type (SELECT) in RADIO.
- Refresh ATC window (ERROR Phase 4).
- QDM TRAFFIC not synchronised 
- Labeling via Traffic manager SID/STAR
- Connecting WORLD servers.
- Saves VOICE check in profile. (Connect)
- Sound "Transfer Request" on autoaccept.
- Set NO-Voice traffic 
- Creating route after receiving FlightPlan sometimes exception.
- NOTAM
- Special Areas
- Traffic speed vector exception error

## [1.2.24.2] - 2022-05-28
### Added
- VOICE ATIS

### Fixed
- Inset traffic refresh exception.
- Hide Alpha choice for beta Staff.
- ATIS configuration voice.
- ATIS screen info
- Show BAY list
- ATIS screen for CTR and FSS
- SID / STAR position data.
- Route time calculation.
- Route Position sid/star.

## [1.2.24.3] - 2022-05-30
### Fixed
- SID / STAR position data.
- Route time calculation.
- Route Position sid/star.
- Double Special Areas.

## [1.2.24.4] - 2022-06-01
### Fixed
- Sid Star Name position.

## [1.2.24.5] - 2022-06-03
### Added
- Highlight labels with middle mouse button.

### Changed
- VOICE ATIS Callsign from data server.

### Fixed
- Direct strange text
- Direct time
- Route time calculation when route is off
- Exam module PDF opening error
- ColorScheme settings after open profile
- MVA when only labels assigned.

## [1.2.24.6] - 2022-06-04
### Added
- SETTINGS/ LABELS MIDDLE MOUSE (Labels MOVE and HIGHLIGHT)

## [1.2.26.0] - 2022-06-05
### Added
- Red UNICOM label in VHF radio form
- Show spinner animation while loading ATIS
- Block connection while sector loading

### Fixed
- Hang on disconnecting
- Test fix for interpolated track
- ATIS spoken twice
- Auto start voice ATIS
- Speak frequency in remarks

## [1.2.26.3] - 2022-06-12
### Added
- Add open full changelog button
- Copy log to clipboard button
- Show columns resizing grab point in ATC window

### Changed
- Airport window columns resizing behavior

### Fixed
- TAB in combitation with PTT shows route
- 3rd party position report closing field
- ATIS loading spinner when observer
- Test fix trainer role check
- Reconnect teamspeak icon high DPI scaling
- Info message box high DPI scaling
- Alpha permission failed check causing downgrade
- Color voice ATIS translation from metar

## [1.2.26.12] - 2022-07-02
### Added
- Allow setting connection port after server address (e.g. worldserver.net.ivao.aero:8609)
- Clear ATIS voice recording button (mock)

### Changed
- Change ATC window resize bar color
- HTTPS TLS version
- High DPI scaling for window control buttons
- Mouse cursor on window buttons
- Vertical radar range up to FL900

### Fixed
- High DPI scaling play sound button, radar symbol, traffic list scroll image 
- Connection menu position relative to cog button
- Local flights as departure when on ground.
- VFR points in route
- MSG label color (EMER,COMMS...)
- Labeling font color to allertcolor 
- Filter and Airport screens resizing
- QDM lines on widescreen
- ATIS window blocked

### Removed
- Connection port

## [1.2.26.17] - 2022-07-24
### Added
- Departure frequency in ATIS

### Changed
- Icons in airport and VHF window are now SVGs to better support high DPI monitors
- ATIS (Voice selection TTS / RECORDING)

### Fixed
- Scrolling filterlist
- QDM window close button
- Voice ATIS wind spelling
- Voice recording ATIS
- Release/Transfer needs to be done twice
- Radio not expanding after made small

### Removed
- Crash handler

## [1.2.26.18] - 2022-07-25
### Added
- Add sections in voice ATIS structure

### Changed
- disable voice atis until ATIS ready

### Fixed
- Background color dynamic labels
- ATIS freq update when changing position

## [1.2.26.19] - 2022-07-27
### Fixed
- Endless atis loading

## [1.2.26.21] - 2022-07-27
### Fixed
- Fix Aurora non launching on some rare occasion

## [1.2.26.22] - 2022-07-28
### Added
- English TTS requirement popup

## [1.3.0.0] - 2022-07-31
### Changed
- SVG drawing mode

## [1.3.0.1] - 2022-08-01
### Fixed
- Application hang on start on Windows 7
- English TTS voice not recognized

## [1.3.0.6] - 2022-08-04
### Fixed
- Wrong credentials using Artifice
- Spec Areas in Inset
- CTD on NaN values in position calculate
- Background frame static labels.

## [1.3.0.8] - 2022-08-08
### Fixed
- Win7 32bits compatible
- DCT time (invisible if not in route)
- Route time miscalculation.

## [1.3.0.9] - 2022-08-11
### Added
- Detailed SSO login error

### Changed
- Voice ATIS is not supported on Windows 7
- Set voice on as default on new installations

### Fixed
- Typo on issue handler window
- Fix CTD if transmitting for more than 30 seconds
- Fix application non starting on Windows 7
- Fix CTD during test voice
- Leading space causes first segment of aicraft route to display wrongly

## [1.3.0.11] - 2022-08-14
### Fixed
- VOR / NDB symbols saved in colorscheme.
- SVG size on some buttons

## [1.3.0.12] - 2022-08-15
### Added
- Intercom SDK

### Fixed
- Fix potential CTD on atis update
- Fix TS2 players context menu not closing

## [1.3.0.14] - 2022-08-17
### Fixed
- UPDATE Beta users.

## [1.3.0.16] - 2022-08-20
### Added
- Traffic voice status SDK
- Get runway configuration of controlled airports with SDK
- Get selected traffic with SDK
- Show changelog button

### Fixed
- Fix unhandled exception logging on non alpha versions

## [1.3.0.17] - 2022-09-03
### Fixed
- Changelog loading slowly
- Empty changelog

### Changed
- Moved custom server port settings to profile.ini

