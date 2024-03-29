# Changelog
## [1.3.0.0] - 2022-08-01
### Added
- Audio compressor to microphone input
- Overhaul windows controls (Maximize, fullscreen, minimize, minimize to tray)
- Message for forced/lost connection
- Super heavy wake turbelence colorscheme support
- Sector loading info on pvd
- CPDLC message filter by response type
- Connection lost message
- Progress bar to update unzip process
- Drag info message window
- Show changelog on startup after update
- Add sector error in Logs\SectorError.log
- Inspection downloaded sectors
- Metric conversion to ATIS TA and TL
- Changed structure on CA / STCA / DUPE
- Responsive buttons in airport window
- Invert MVA and VFR buttons in airport window
- Traffic QDM can turn 360 degrees
- Auto update QDM manager data while window is open
- Send text button in traffic manager
- Allow running only one instance of Aurora
- New SSO login system
- Logout button
- User account window
- Shadow to windows
- Resize on left border of main window
- Red UNICOM label in VHF radio form
- Show spinner animation while loading ATIS
- Block connection while sector loading
- Highlight labels.
- Departure frequency in ATIS
- English TTS requirement popup
- VOICE ATIS


### Changed
- Better tooltips
- Pretty format control session recordings
- Zoom smoothness
- Improved tfl drawing performance when zoomed in
- Increased extrapolated track threshold
- Moved QDM data further away from cursor
- Send pm button in traffic manager now opens PM in comm box
- Airport window columns resizing behavior
- High DPI scaling for window control buttons
- Vertical radar range up to FL900
- SVG drawing mode to better support high DPI monitors

### Fixed
- Speed unit conversion
- Overlapping traffic label (last selected traffic stays on top)
- Names column disappearing from inset transfer list
- Duplicate keyboard shortcuts
- Save/load DEFA areas
- Nav aids label position
- Traffic visibility filter inset
- Notams in inset
- CPDLC window not expanding if saved as when collapsed
- Improved 3rd party stability
- Exam module PDF opening error
- TAB in combitation with PTT shows route
- Local flights as departure when on ground.
- Release/Transfer needs to be done twice
- Radio not expanding after made small
- Background color dynamic labels

### Removed
- Bold from free text and bay inputs

## [1.3.0.1] - 2022-08-01
### Fixed
- Application hang on start on Windows 7
- English TTS voice not recognized

## [1.3.0.6] - 2022-08-06
### Fixed
- Wrong credentials using Artifice
- Spec Areas in Inset
- CTD on NaN values in position calculate
- Background frame static labels.

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
- Win7 32bits compatibility issue
- DCT time (invisible if not in route)
- Route time miscalculation

## [1.3.0.11] - 2022-08-14
### Fixed
- VOR / NDB symbols saved in colorscheme.
- SVG size on some buttons

## [1.3.0.14] - 2022-08-18
### Added
- Intercom SDK

### Fixed
- Fix potential CTD on atis update
- Fix TS2 players context menu not closing

## [1.3.0.17] - 2022-09-03
### Fixed
- Changelog loading slowly
- Empty changelog
- Traffic voice status SDK
- Get runway configuration of controlled airports with SDK
- Get selected traffic with SDK
- Show changelog button

### Changed
- Moved custom server port settings to profile.ini
- Fix unhandled exception logging on non alpha versions


## [1.3.0.19] - 2022-09-15
### Fixed
- Autorisation data (internal change)
- Star linetype on startup
- Sector drawing issue on some geometries with negative coordinates

### Changed
- Accepts all windows voices for voice ATIS

## [1.3.0.33] - 2023-05-08

### Fixed.
- Issue forcing antenna position always on airport center point
- ft in transition altitude when mtr is assigned.
- ATIS open screen blocked for a few sec.
- Issue forcing antenna position always on airport center point
- Crashing on svg (images) viewer
- PTT buffer error
- Trainers / examiners receiving ATIS in sequense.
- Extra navaid info on route.
- Missing/double nav data on route
- Transferlist invisible on high dpi
- Change EOBT via stripslist.
- CPDLC/TELEX sending strange values on hoppie.nl.
- CPDLC / DCL losing assinged data.
- Cancel next ATC
- Callsign in Guard message

### CHANGED
- PTT block time increased for ATC
- ATIS selects auto english tts.
- Sort alphabetic transferlist.
- Nearest airport in INSET skips hiden
- Block ATIS if offline.
- ACC lines drawing above HS and LS


### ADDED
- Sector : Voice ATIS structure on atc positions.
- Colorscheme : Line type for airways.
- Transfer list in call history intercom.




