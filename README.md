# Breezefen 1.0 TEST
Native Android Four Winds straight-arm cover puzzle. Android8+ (min26), target35. Package com.gg007.breezefen.

## Rules
Four Winds: fixed numbered hubs extend straight arms up, right, down or left. Each hub number is the combined length of its arms, excluding the hub itself. Directions may stay empty. Every empty cell must be covered by exactly one arm. Arms cannot overlap, cross, bend, leave the grid or pass another numbered hub. Select a hub, then tap an aligned endpoint to set that arm. Tap the same endpoint again to erase it. Undo/reset/next/levels and saved wind palette/hub-usage labels. Twelve unique 4x4 hub layouts and unique solutions.

## Download and status
https://mega.co.nz/#!8MlQxIAY!QRGmI9GklPcuUh5cvbhjb0tWZgy6Yujj4WMtnpfB_N8
APK SHA256 d66dddfbc4e10d8e1849ba5a19de85d853ccd81fcf838a9a7877af02366dda52; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous download bytes match.

## Checks
Independent coordinate-list/set oracle agrees with production step-walk/bitmasks for all316192 partial arm-shape combinations,120000 invalid/random states and1152 ray boundary cases. Every board has one solution; hub layouts and solutions are distinct. At least two hubs split into multiple arms in each solution; each hub has at least two geometrically possible exact-total shapes before non-overlap constraints. Bounds, invalid levels/directions/array sizes, solved lock, solve/undo/reverse-order replay pass. Actual archived generator regeneration and Java tests pass. Drawing-adapter hub/endpoint set-erase/undo, menu/settings/privacy/levels/next and saved preference/completion checks pass. Actual game/solved/menu/settings/privacy/levels drawing pixels inspected, not phone screenshots. Phone runtime, performance and external-browser handoff QA remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Live803-entry registry,123 recovered partial READMEs and semantic review of all149 prior studio cards found no Four Winds match. Homebriar moves each circle once by its fixed distance and assigns one arrival to each country; it does not cover every empty cell or split lengths over arms. Compassfern grows connected regions with N/E/S/W area counts, including off-axis cells. Breezefen instead splits one total over straight rays from each fixed hub, covering all non-hub cells exactly once. Known Four Winds genre, not a global invention; recovered corpus is partial. Rules https://wpcunofficial.miraheze.org/wiki/Four_Winds https://wiki.logic-masters.de/index.php/Four_Winds/en https://pleasantpuzzles.blogspot.com/2022/10/puzzle-213-four-winds.html .

## Build
JDK17 and AndroidSDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. Board.java embeds generated hubs/totals/solutions. javac -d /tmp/breeze-test src/com/gg007/breezefen/Board.java BoardTest.java and java -cp /tmp/breeze-test com.gg007.breezefen.BoardTest. bash build.sh creates an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to private original signing inputs. No credentials in source. Release build settings, signed TEST artifact, not final store release.

## Privacy and branding
Breezefen runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Wind palette, hub-usage labels and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 icon byte-equal to original. Menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and websites
Complete source and APK privately preserved at https://files.instinct.com/7rwqv2nhek5u-breezefen-source-archive, including exact cumulative150-card studio and published catalog/studio sources/updater. Repository https://github.com/iLanis-agent/breezefen holds README only; full Git source commit pending. Both website publications checked separately. No Pages settings change or Play rollout. November7,2026.
