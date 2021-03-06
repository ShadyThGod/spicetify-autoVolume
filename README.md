# spicetify-autoVolume
Extension for spicetify-cli which automatically decreases volume at specific intervals of time.

### Why?
I've made this extension for people who listen to music for long periods of time and care about their ears. This extension, when enabled using the toggle in the menu, automatically decreases the volume by a specific percentage at specific intervals of time until the volume reaches a specified minimum percentage. This way, you can listen to music for long time and making sure you're not hurting your ears much.

If you're someone who listens to music for long periods of time, I really recommend this. Your hearing matters!

## Requirements
- Make sure you have installed spicetify-cli ([instructions here](https://github.com/khanhas/spicetify-cli/wiki/Installation)) and generated config ([instructions here](https://github.com/khanhas/spicetify-cli/wiki/Basic-Usage))

## Installation
- Download [autoVolume.js](https://github.com/amanharwara/spicetify-autoVolume/raw/master/autoVolume.js)
- Copy/move the file to any of the following:
  - `Extensions` folder in Home directory:
    - Windows: `%userprofile%\.spicetify\Extensions\`
    - Linux: `$XDG_CONFIG_HOME/.config/spicetify/Extensions/ or ~/.config/spicetify/Extensions`
    - MacOS: `~/spicetify_data/Extensions`
  - `Extensions` folder in Spicetify executable directory.
- Run command: `spicetify config extensions autoVolume.js` (Adds autoVolume.js to the config)
- Apply using either of the commands:
  - `spicetify backup apply`
  or
  - `spicetify apply`

## Changing the interval/minimum volume

### To change the percentage to decrease the volume by
- Open `autoVolume.js` in an editor of your choice.
- Find the line `const DecreaseBy = 5;`
- The value is in percentages, so change the '5' to any percentage you want.
- Save the file.
- Run the command `spicetify apply` to apply the changes.

### To change the interval

- Open `autoVolume.js` in an editor of your choice.
- Find the line `const interval = 5;`
- The interval value is in minutes, so change the '5' to any amount of minutes you want.
- Save the file.
- Run the command `spicetify apply` to apply the changes.

### To change the minimum volume

- Open `autoVolume.js` in an editor of your choice.
- Find the line `const minimumVolume = 50;`
- The minimum volume value is in percentage, so change the '50' to any percentage of volume that you want.
- Save the file.
- Run the command `spicetify apply` to apply the changes.

## Usage
Toggle "Auto Volume" in the profile menu.

![autoVolume Screenshot](https://github.com/amanharwara/spicetify-autoVolume/raw/master/autoVolume-screenshot.png)

### While you're at it, make sure to check out the **[Make Listening Safe](https://www.who.int/pbd/deafness/activities/MLS/en/)** campaign by the World Health Organization. It has much more information about the effects of noise and what can you do to ensure you are listening safely.
### Also check out the [Reading Material](https://github.com/amanharwara/spicetify-autoVolume/wiki/Reading-Material) section of the wiki for more links related to the subject.
