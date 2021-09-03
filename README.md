# bottom-sheet-issue
Project demonstrates BottomSheet issue that was introduced in Material Components 1.4.0 release

https://github.com/material-components/material-components-android/releases/tag/1.4.0

Issue: https://github.com/material-components/material-components-android/issues/2358

# WTR
1. Rotate device to landscape (screen width should be more than 640dp – see `material_bottom_sheet_max_width` dimen from material-components resources).
2. Press the button
3. Roate device back to portrait mode.

# Expected behavior
BottomSheet width is invalidated and fit the screen even if activity is not recreated on orientation change.

# Actual behavior
BottomSheet width doesn't change, its content is clipped.

<img src="https://github.com/enginegl/bottom-sheet-issue/blob/master/img/landscape.png?raw=true" width="456" height="216">
<img src="https://github.com/enginegl/bottom-sheet-issue/blob/master/img/portrait.png?raw=true" width="216" height="456">
