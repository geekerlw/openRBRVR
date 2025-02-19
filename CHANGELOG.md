## 0.6.0

- Implement per-stage supersampling
- Change config file format from ini to toml
- Add overlay adjustment menu. Show overlay borders while driving when debug
  mode is active for easier adjustment.
- Attempt to fix intermittent recentering issues happening with Reverb in
  OpenXR mode.

## 0.5.2

- Do not crash the game if a VR headset is not connected
- Fix a bug in horizon lock amount loading and adjustment

## 0.5.1

- SteamVR: Improve concurrent Vulkan queue usage
- Make the amount of correction that lock to horizon applies adjustable

## 0.5.0

- Implement OpenXR support
- Change internal GPU synchronization logic

## 0.4.5

- Fix tracking lag that occurred for some Oculus users.
- Fix particle rendering issue where too much of the particles were visible
  inside the car cockpit.

## 0.4.4

- Changes to potentially improve the stability of the plugin.
- Fix black opaque square being rendered in front of the car in external
  cameras if "render car shadows" was active.

## 0.4.3

- Combine previous cockpit rendering detection logics. They both have issues
  with certain cars so both are now used to minimize car rendering issues.
- Fix a logic bug with "Always call Present" debug option that rendered it useless.

## 0.4.2

- Change the logic how cockpit rendering is detected. Fixes a rendering issue
  with Skoda Fabia R5.
- Change "Show desktop window" logic in a way that the desktop window rendering
  is disabled only when driving mode is active.

## 0.4.1

- Use correct aspect ratio from desktop window size for 2D planes.
- Add "Render replays in 3D" option.
- Add "Always call Present" debug option to the debug menu.

## 0.4.0

- Add support for anti-aliasing and anisotropic filtering
- Tweak stage rendering to reduce object clipping on close contact
- Improve internal error handling
- Renew the Options -> Plugins -> openRBRVR menu

## 0.3.1

- Fix main menu clipping too early
- Fix desktop window color rendering

## 0.3.0

- Fix black screen in front of the windshield if Pacenote plugin is not active
- Fix car interior clipping too early when getting close to it
- Fix trackside object flickering (in Antaramanana for example)
- Pause menu is now rendered over 3D content by default. 3D rendering can also
  be toggled on for the spinning camera and main menu. Thanks for @dancek for
  the contribution.

## 0.2.0

- Loading screen can now be toggled off
- `openRBRVR.ini` can now be written from the in-game options menu
- Overlay (digidash etc.) is now fixed to the car's rotation also in
  lock-to-horizon mode

## beta9

- Fix RBRHUD + BTB stage rendering issue
- Internal improvements

## beta8

- Fix crashes when loading certain BTB stages

## beta7

- Fix skybox and fog rendering

## beta6

- Add drawDesktopWindow option to openRBRVR.ini. Drawing of the desktop window can be disabled with this. The option is also available from Options -> Plugins -> openRBRVR
- Make overlay (the 2D content while driving) position fully adjustable. openRBRVR.ini keys overlayTranslateX, overlayTranslateY and overlayTranslateZ can be used to translate the overlay.

## beta5

- Fix rendering issues on Ahvenus I, Ahvenus II and Pirttikulma
- Fix an issue where the stuttering remained on stage once it had started

## beta4

- Render view from the left eye is on the desktop window
- Add better frame time debug information when debug mode is active
- Support lock to horizon for roll and pitch axes or both

## beta3

- Add support for displaying debug information
- Create openRBRVR.ini if it's missing
- Handle ASLR correctly

## beta2

- Fix an issue where the license text page crashed the game

## beta1

- First public beta of openRBRVR
