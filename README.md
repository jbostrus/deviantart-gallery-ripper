# deviantart-gallery-ripper
Click button and generate a list of direct image link urls for all images for a users gallery.

# TOC 
* [Function](#function) - explanation of script
* [Usage](#usage) - detailed usage example
* [Known Issues](#known-issues) - list of known problems with script usage
* [Change Log](#change-log) - details of changes between versions

# Function
Utility script to assist with downloading mass images from a DeviantArt gallery.
The script generates a textbox with direct image link urls at the top of a gallery page. Copy and paste the urls into download manager of choice. Tested and works best with [DownThemAll](https://addons.mozilla.org/en-US/firefox/addon/downthemall/) add-on for FireFox. Sample custom filter to select download links `[pre??.deviantart.net/,orig??.deviantart.net/,img??.deviantart.net/]`

# Usage
* Open a gallery page on DeviantArt website. There will be a small button under the deviant art logo. Click it to start fetching the image links. 
  * ![img](http://i.imgur.com/mYsrmSb.png)
* Depending on the number of gallery pages it may take some time to parse it all out.
  * ![img](http://i.imgur.com/xKDH4Cf.png)
* Once completed there will be a textbox containing a list of direct download links for each of the images.
  * ![img](http://i.imgur.com/jXmlU18.png)
* In the case of problems you may get an error list. This is usually because some of the pages had no images associated with it. For example story only posts, PDF, Flash, or SWF pages. You may copy/click the link to open the offending page to review.
  * ![img](http://i.imgur.com/jXmlU18.png)

# Known Issues
* When browsing a search/gallery and clicking a thumbnail to load full image on HTML5 browsers the GET button disappears. This is because DA hides the panel holding the button. Refreshing the page while viewing the single image will redraw the GET button allowing you to grab all images in the image artist's gallery.

# Change Log
v1.0.19
* user contribution: Added automatic text box selection when finished.
v1.0.20
* Extended textbox of urls to fill the frame when completed.
* Added ignore code so it won't draw the download button on some pages where it cannot get a gallery list.
* Fixed iframe code for dev mode Chrome so it can work again instead of crashing the javascript vm.
