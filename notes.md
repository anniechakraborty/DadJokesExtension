# Code Explanation and Pointers

## Significance of manifest.json
- We define the properties of our extension in _manifest.json_ . 
- In these properties we can define the name of the extension, version and manifest_version. (The manifest_version : 2 has been depreciated from this year onwards. Use the manifest_version : 3 instead.)
- Defining these properties will create our extension. We can directly load this json in chrome.

## Loading an extension
- Go to the Chrome browser. Open extensions.
- Switch on the Developer mode.
- Click on "Load Unpacked" button and select the folder containing the manifest.json file. This will create our extension which is right now bare bones.

## Adding functionality to the extension
- In manifest.json we add a new key "browser_action" which takes in a dictionary with the following keys and values:
    - "default_popup" : "popup.html", // the file containing the logic
    - "default_icon" : "logo.png", // the logo sixe should be 128 X 128 pixels
- In manifest.json we can also add permissions such as "activeTab" (_TODO : Read about the permissions availale which can be given in an extension_) and icons where we can define the icon pngs for different sizes.

