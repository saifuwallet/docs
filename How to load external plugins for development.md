# How to load external plugins for development
🚧 The plugin system is changing rapidly, this page might not be up to date 🚧 

**Note:** Due to sandbox restrictions this will only work in Chrome

## Preparing Saifu
1. Download the latest chrome dev build (coming soon)
2. Navigate to your browsers extension settings and enable 'Developer mode' in the top right corner
![](attachments/Screen%20Shot%202022-03-31%20at%2012.13.14.png)
3. Click 'Load unpacked' 
4. Navigate to the unpacked folder containing the Saifu dev version

If all worked fine, Saifu should load successfully

![](attachments/Screen%20Shot%202022-03-31%20at%2012.15.09.png)

## Loading plugins for development

Inside the saifu folder, navigate to the folder `plugins`, or create it if it doesn't exist yet. 

Create a new sub-folder with your plugin name and copy the contents of your built plugin bundle (manifest.json + main.js)

![](attachments/Screen%20Shot%202022-03-31%20at%2012.16.30.png)

On next open, Saifu will attempt to load your custom bundle. Navigate to the plugin settings and enable it

![](attachments/Screen%20Shot%202022-03-31%20at%2012.18.05.png)

### Hints:
- Symlink or setup your plugin environment to automatically generate these files and put them into the right place
- Inject sourcemaps into the bundle for easier development 