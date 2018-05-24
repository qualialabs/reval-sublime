## Meteor Reval - Instant Reloading with Sublime & Meteor

This plugin is for use in combination with [Reval](https://github.com/qualialabs/reval) to allow for instant reloads with Meteor.

### Meteor Setup

1. Install the Atmosphere package `meteor add qualia:reval`

### Sublime Global Setup

1. Install [Sublime Package Manager](https://packagecontrol.io/installation)
2. Type "command + P" then type "Install Package" into prompt
3. Type "Meteor Reval"
4. Configure User Settings in `Preferences -> Package Settings -> Meteor Reval`

### Sublime Per-Project Setup

You can specify settings in your `.sublime-project` file to modify the host name for each project using reval
* Add a block in your `.sublime-project` with overrides for the project like
```json
	"settings": {
		"meteor_reval": {
  		"reload_on_modified" : true,
		  "hostname": "some.hostname",
		  "required_path": "\\\\Special\\Path",
		  "path": "\\\\Full\\Path\\To\\App",
		}
	}
```

## How to Develop

1. Download zip file of this repo
2. Extract to your `Packages/MeteorReval`
3. Remove any existing version installed from package control
4. Reload Sublime. Sublime will now use the local package in `Packages/`
5. Make modifications locally to `MeteorReval.py`

Package Folder Location
* Windows: `%APPDATA%\Sublime Text 3`
* OS X: `~/Library/Application Support/Sublime Text 3`
