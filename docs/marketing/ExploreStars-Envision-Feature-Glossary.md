# ExploreStars Envision Feature Glossary

## Legacy ExploreStars + Envision Shared Features

The features in this section are available in both the legacy ExploreStars app and the new ExploreStars Envision app. Envision preserves these core telescope-control workflows while presenting them in a modernized interface and, in several cases, expanding the surrounding tools.

| # | Feature | Explanation |
|---:|---|---|
| 1 | Mount Connection | Both legacy ExploreStars and Envision connect to PMC-Eight telescope mounts so the software can send control commands. Envision preserves this core role while expanding the available connection options. |
| 2 | WiFi Mount Control | Both apps support WiFi communication with PMC-Eight mounts. This remains the primary wireless control method shared between legacy ExploreStars and Envision. |
| 3 | Serial / USB Mount Control | Both apps can support direct wired mount communication where the platform and hardware allow it. Envision continues this capability through serial or USB COM-port operation on supported systems. |
| 4 | Virtual Alignment Mount Model Selection | Both apps require the user to select the mount model so the software can apply the correct virtual alignment behavior. Envision carries this forward with model presets for supported PMC-Eight mounts. |
| 5 | Site Latitude | Both apps use observing latitude for pointing and sky calculations. Envision keeps this setup field and ties it into live telemetry and visibility tools. |
| 6 | Site Longitude | Both apps use observing longitude to calculate local sky position. Accurate longitude remains essential for GoTo, tracking, and target visibility. |
| 7 | Local Time | Both apps depend on correct time for astronomical calculations. Envision makes local time more visible as part of the setup and telemetry workflow. |
| 8 | Local Sidereal Time | Both apps use local sidereal time for celestial coordinate conversion. Envision displays LST prominently so users can monitor it during observing. |
| 9 | Object Catalog | Both apps provide access to astronomical object catalogs. Envision preserves catalog-based observing while expanding search and object-detail tools. |
| 10 | Catalog Search | Both apps let users search for catalog objects by name or designation. Envision modernizes this with faster, richer target lookup behavior. |
| 11 | Target Selection | Both apps let the user select a target before commanding the mount. Envision adds more supporting target information around the selected object. |
| 12 | Target Coordinates | Both apps display celestial coordinates for selected targets. Envision expands this with RA, Dec, Alt, Az, and related live context. |
| 13 | Solar System Targets | Both apps support selecting major solar-system objects. Envision improves this with clearer altitude/status handling and current-position calculations. |
| 14 | GoTo | Both apps can slew the mount to a selected target. Envision keeps GoTo central while adding more workflow options around what happens afterward. |
| 15 | Sync | Both apps allow the user to synchronize the mount position to a known target. This improves pointing accuracy after centering an object. |
| 16 | Manual Slewing | Both apps allow direct manual movement of the mount. Envision implements this through the Control page and thumb pad controls. |
| 17 | Direction Controls | Both apps provide directional movement controls for centering and framing. Envision adds live mount and target readouts around these controls. |
| 18 | Slew Rate Control | Both apps let users adjust how fast the mount moves during manual slews. Envision presents this through clearer fine and coarse rate controls. |
| 19 | Tracking Control | Both apps can start or stop mount tracking. Envision preserves this core mount-control function in a dedicated tracking panel. |
| 20 | Connection Status | Both apps indicate whether the mount is connected. Envision keeps connection state visible in the app bar and telemetry area. |
| 21 | Night-Friendly Operation | Both apps are intended for use at the telescope under dark-sky conditions. Envision expands this with a dedicated night vision mode. |

## New Or Expanded In Envision

The features in this section are new to Envision or significantly expanded compared with the legacy ExploreStars app. They reflect Envision's broader connectivity, modern interface, richer charting tools, and enhanced virtual alignment capabilities.

| # | Feature | Explanation |
|---:|---|---|
| 22 | Bluetooth Mount Control | Bluetooth mount control is newly added in Envision and is not supported by the legacy ExploreStars app. It allows compatible devices to connect to supported PMC-Eight systems without using the PMC-Eight WiFi network. |
| 23 | Modern App Bar | Envision adds a persistent top app bar for help, night mode, branding, and connection state. This gives the app a more modern and consistent user interface. |
| 24 | Telemetry Strip | Envision adds a persistent telemetry strip for RA, Dec, LST, Alt, Az, hour angle, and mount status. This keeps live observing information visible across workflows. |
| 25 | Bottom Navigation Bar | Envision adds a modern bottom navigation model. It makes Setup, Target, Visibility, Control, Log, and Star Seeker easy to reach. |
| 26 | Display Language Selection | Envision adds multilingual display support. Users can select the UI language, with untranslated text falling back to English. |
| 27 | GPS Location Fill | Envision can request device location and fill in observing coordinates when supported. This reduces setup friction and avoids manual coordinate entry errors. |
| 28 | Nearby Search | Envision adds a search mode for objects near the current mount position or selected area. This helps users discover nearby targets during a session. |
| 29 | Saved Targets | Envision adds a saved-target workflow for custom or frequently used targets. This helps users build and reuse a personal observing list. |
| 30 | Custom Coordinate Dialog | Envision adds structured manual entry for custom RA/Dec targets. It supports named targets and coordinate epoch handling. |
| 31 | J2000 / JNOW Handling | Envision lets users specify whether entered coordinates are J2000 or current epoch. This improves accuracy when using coordinates from different sources. |
| 32 | Alt/Az GoTo | Envision adds direct horizon-coordinate GoTo. Users can command the mount using altitude and azimuth instead of RA/Dec. |
| 33 | Visibility Page | Envision adds a dedicated page for target observability. It shows altitude, visibility status, and timing information for the selected object. |
| 34 | Wikipedia Lookup | Envision can open object information from Wikipedia when online. This adds educational context directly to the observing workflow. |
| 35 | Image Thumbnails | Envision shows target image thumbnails when available. Users can open a larger view for visual reference. |
| 36 | Star Seeker Sky Chart | Envision adds the built-in Star Seeker chart. It provides an offline planetarium-style view inside the app. |
| 37 | FREE Chart Mode | Envision's Star Seeker includes a free navigation mode for exploring the chart manually. This allows sky browsing without locking to the mount. |
| 38 | LIVE Chart Mode | Envision's Star Seeker can follow the current sky or mount context. This gives users a live chart view tied to observing conditions. |
| 39 | Push-To Mode | Envision adds push-to style operation through Star Seeker. This supports manually guided observing workflows in addition to motorized GoTo. |
| 40 | Mount Marker / Telrad Overlay | Envision adds visual overlays showing mount position and finder-style aiming aids. These make the chart more useful at the telescope. |
| 41 | Solar-System Chart Bodies | Envision displays solar-system bodies directly in Star Seeker. This connects planetary observing with the same interactive chart used for stars and deep-sky objects. |
| 42 | Magnitude Slider | Envision lets users adjust chart object visibility by magnitude. This improves chart readability for different skies, devices, and observing goals. |
| 43 | Reference Lines & Zenith | Envision adds chart overlays such as reference lines and zenith indicators. These help users orient themselves in the sky chart. |
| 44 | Object Identification | Envision supports tapping or selecting objects in Star Seeker for identification. This turns the chart into an interactive observing and learning tool. |
| 45 | Mirror Mode / Star Diagonal | Envision supports chart mirroring for diagonal or optical-view matching. This helps the screen match what the observer sees at the eyepiece. |
| 46 | Equatorial / Alt-Az Chart Modes | Envision supports chart behavior appropriate to equatorial and alt-az contexts. This improves usability across different mount configurations. |
| 47 | Coordinate Grids | Envision adds configurable chart grids. These improve orientation and make the chart more useful for locating objects. |
| 48 | Chart Settings | Envision includes dedicated chart configuration. Users can tailor Star Seeker to observing preferences and display needs. |
| 49 | Offline Chart Data | Envision emphasizes offline catalog and chart operation. This is important for field use where internet access may be unavailable. |
| 50 | Firmware Config | Envision exposes firmware configuration as a connected tool. It brings controller setup closer to the main observing workflow. |
| 51 | Astronomy Calculators | Envision includes built-in astronomy and optics calculators for common observing setup tasks. These tools help users estimate values such as field of view, magnification, and other telescope/eyepiece relationships without leaving the app. |
| 52 | Enhanced Virtual Alignment Mount Modeling | Envision adds an enhanced virtual alignment mount modeling tool based on a seven-star alignment model. The model provides pointing corrections for polar alignment error, home-position error, mount leveling error, cone angle, and related mechanical or setup offsets. |
| 53 | Star Alignment | Envision includes a dedicated multi-star alignment workflow. This helps improve mount pointing accuracy after setup and supports the virtual alignment model. |
| 54 | Daylight Polar Alignment | Envision adds a daylight polar-alignment tool. This gives users a specialized setup aid before nighttime observing. |
| 55 | Meridian Flip Control | Envision exposes meridian flip behavior as a user-facing control panel. This is especially useful for German equatorial mount operation. |
| 56 | Spiral Search | Envision adds an integrated expanding-pattern search tool. It helps locate objects that are near but not centered in the eyepiece or camera field. |
| 57 | Log Page | Envision includes a dedicated log screen for application and connection activity. This helps users diagnose setup, connection, and control issues. |

## Summary

ExploreStars Envision retains the core telescope-control functions users know from legacy ExploreStars: mount connection, WiFi control, model selection, target selection, GoTo, Sync, manual slewing, tracking, and night-friendly observing support. Envision then expands the platform with Bluetooth connectivity, a modern multi-page interface, persistent telemetry, Star Seeker charting, push-to observing, richer target tools, astronomy calculators, and an enhanced seven-star virtual alignment mount modeling system.
