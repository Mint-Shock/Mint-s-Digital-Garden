- [ ] Main Toggle
	- [x] General Disable
	- [ ] Temp Auto Disable
		- `Switcher-Cutout/13-Bool`
		- [ ] if no user is being cutout
			-  `Switcher-Cutout/1-bool` ^c7van
		- [ ] if current camera is of a Type that should be disabled
			- 

---

- [ ] Change cutout background color 
	- `Switcher-Cutout/8-Int` ^zyqw9
		- Index of Active Color
	- [ ] Background color
		- [x] `0` 🌈 Custom color
			- **Component**: ButtonEditColorX
				- `Switcher-Cutout/4-colorx` ^gsvaw
		- [x] `1`⚪ Transparency switch ^1m02t
			- ==Needs mod to work:== https://github.com/art0007i/TransparentCameraEnabler 
		- [x] Color Presets
			- [x] `2` 🔴 Red - FF0000 ^q-d74
			- [x] `3` 🟡 Yellow - FFFF00 ^o2nk7
			- [x] `4` 🟢 Green - 00FF00 ^207yy
			- [x] `5` ♏ Mint - 00FFFF ^ce6cx
			- [x] `6` 🔵 Blue - 0000FF ^7b88a
			- [x] `7` 🟣 Purple - FF00FF ^nglpw
			- [x] `8` ⚫ Black - 000000 ^gaapy
			- [x] `9` 🔘 Gray - 808080 ^aztfw
			- [x] `10` ⚪ White - FFFFFF ^64ohd
		- [?]  `11` 🅰️ Automatic Color selector for Cutout ^rhz3f
			- [?] Use Raycasts to scan image
			- https://discord.com/channels/1248240128942411828/1248259076983488515/1359028435653230784

---

- [ ] Main User
	- [x] Enable / Disable Cutout
		-  `Switcher-Cutout/2-bool` ^002mm
	- [x] Select user from Username
		- [x] Textbox ^na2-9
	- [ ] Radial ui
		- [ ] Toggles
			- [ ] Main Toggle  [[Reso Cutout Stream Vtube Camera#^c7van]]
			- [ ] Toggle Main User [[Reso Cutout Stream Vtube Camera#^002mm]]
			- [ ] Toggle extra devices [[Reso Cutout Stream Vtube Camera#^ad2gq]]
			- [?] Toggle named users
		- [ ] Color Presets:
			- [ ] 🌈 Color Selector [[Reso Cutout Stream Vtube Camera#^gsvaw]]
			- [ ] ⚪ Transparent [[Reso Cutout Stream Vtube Camera#^1m02t]]
			- [ ] 🔴 Red [[Reso Cutout Stream Vtube Camera#^q-d74]]
			- [ ] 🟡 Yellow [[Reso Cutout Stream Vtube Camera#^o2nk7]]
			- [ ] 🟢 Green [[Reso Cutout Stream Vtube Camera#^207yy]]
			- [ ] ♏ Mint [[Reso Cutout Stream Vtube Camera#^ce6cx]]
			- [ ] 🔵 Blue [[Reso Cutout Stream Vtube Camera#^7b88a]]
			- [ ] 🟣 Purple [[Reso Cutout Stream Vtube Camera#^nglpw]]
			- [ ] ⚫ Black  [[Reso Cutout Stream Vtube Camera#^gaapy]]
			- [ ] 🔘 Gray [[Reso Cutout Stream Vtube Camera#^aztfw]]
			- [ ] ⚪ White [[Reso Cutout Stream Vtube Camera#^64ohd]]
			- [?] 🅰️ Automatic Color [[Reso Cutout Stream Vtube Camera#^rhz3f]]

---

- [ ] User devices
	- [x] Enable / disable cutout
		- `Switcher-Cutout/3-bool` ^ad2gq
	- [ ] Make standard models
		- [ ] Microphone 
			- [ ] Add switch to enable and disable
			- [ ] Using key bind or Button on the Model for toggle
			- [ ] Main User can make public
		- [ ] Balloon 
			- [ ] Always point upwards
		- [x] Cookie
			- [x] Use avali cookie
	- [x] Holding in Hand
	- [x] Adding to Toolshelf
	- [ ] System to register microphones with slot input / putting items onto a shelf and them being added

---

- [?] Extra named users
	- [?] Enable / disable cutout
	- [?] Create User List
		- [?] Add User
			- [?] Button that gets username of clicking user
			- [?] Manual input
		- [?] Remove User

---

- [ ] Temp Auto Disable System if no user is selected
	- [ ] What to check:
		- [ ] Main User 
			- [x] Toggles on
			- [ ] user with that username has been found
		- [x] User devices
			- [x] Check if any of the devices finds a user
		- [?] Named Users
			- [?] Check all Toggles
			- [?] Check if any users have been found

---
- [ ] Temp Auto Disable System on specific Camera Type
	- If the current camera (found by comparing the Slotname of the parents of `Switcher/1-Slot`) Should be Disabled. Disable System.
		- [ ]  Static ^7sk1e
			- `Switcher-Cutout/9-bool`
		- [ ] POV ^i4qw1
			- `Switcher-Cutout/10-bool`
		- [ ] TPFV (Third person front view) ^3-28q
			- `Switcher-Cutout/11-bool`
		- [ ] TPBV (Third person back view) ^b0ipq
			- `Switcher-Cutout/12-bool

---

- [?] User Overlay on Camera (Picture in Picture)
	- Add extra Camera that renders to a transparent Plane that gets moved in front of the camera
	- Not visible to users only to camera?

---

- [ ] Ui - Horizontal Layout
	- [ ] `0` Toggle System Main [[Reso Cutout Stream Vtube Camera#^c7van]]
	- [ ] `1` Auto Disabled by camera Type and or Auto disabled because no user is selected.
	- [x] `2` Toggle Main User [[Reso Cutout Stream Vtube Camera#^002mm]]
		- [x] Input Main Username manually[[Reso Cutout Stream Vtube Camera#^na2-9]]
		- [ ] Button that takes Username from whoever pressed it
	- [x] `3` Toggle extra user devices [[Reso Cutout Stream Vtube Camera#^ad2gq]]
	- [ ] `4` Auto Diable Camera Type
		- [ ] Static [[Reso Cutout Stream Vtube Camera#^7sk1e]]
		- [ ] POV [[Reso Cutout Stream Vtube Camera#^i4qw1]]
		- [ ] TPFV (Third person front view) [[Reso Cutout Stream Vtube Camera#^3-28q]]
		- [ ] TPBV (Third person back view) [[Reso Cutout Stream Vtube Camera#^b0ipq]]
	- [ ] `5` --- Spacer ---
	- [?] `6` Named Users
		- [?] Toggle named users 
		- [?] Display all named Users
		- [?] Add / Remove Named Users 
			- [?] Profile picture
				- **Component**: CloudUserInfo
				- https://wiki.resonite.com/Component:CloudUserInfo
	- [?] `7` --- Spacer ---
	- [x] `8` Pick Color [[Reso Cutout Stream Vtube Camera#^gsvaw]]
	- [x] `9` Toggle Cutout/Transparency [[Reso Cutout Stream Vtube Camera#^1m02t]]
	- [ ] `10`Preset Colors - Grid layout
		- [ ] 🔴 Red [[Reso Cutout Stream Vtube Camera#^q-d74]]
		- [ ] 🟡 Yellow [[Reso Cutout Stream Vtube Camera#^o2nk7]]
		- [ ] 🟢 Green [[Reso Cutout Stream Vtube Camera#^207yy]]
		- [ ] ♏ Mint [[Reso Cutout Stream Vtube Camera#^ce6cx]]
		- [ ] 🔵 Blue [[Reso Cutout Stream Vtube Camera#^7b88a]]
		- [ ] 🟣 Purple [[Reso Cutout Stream Vtube Camera#^nglpw]]
		- [ ] ⚫ Black  [[Reso Cutout Stream Vtube Camera#^gaapy]]
		- [ ] 🔘 Gray [[Reso Cutout Stream Vtube Camera#^aztfw]]
		- [ ] ⚪ White [[Reso Cutout Stream Vtube Camera#^64ohd]]

---

- [ ] Privacy
	- [ ] Respect settings from Multicam settings
	- [ ] Override on user devices to be able to give them to users that don't have permission

