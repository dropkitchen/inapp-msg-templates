# inapp-msg-templates
custom artwork message  templates that can be used with localytics in-app messaging

# Localytics - In-App Message Templates

___

##### To create a center modal in-app message use the following:

- For iphone download the folder [iphone-center-modal-template]
- For iPad download the folder [ipad-center-modal-template]
___

Inside this folder you will find a file called [index.html].
Within this file you will need to edit the following: 

  - Title
  - Message
  - Button text

#### To edit the **Title** of your in-app message:
Enter your text between the 

`<h1></h1>` tags.

>Eg. `<h1>WWWWWWWWW</h1>` Replace `WWWWWW` with your text.

#### To edit the **Message**
Enter your text between the `<div id="message"></div>` tags.

>Eg. 
    ```<div id="message">
        Apple pie sweet......
    </div>```
Replace ```Apple pie sweet.....```
    
### To edit the text within the **buttons**

1. For the **dismiss button** replace the text between `<button id="red_button></div>` tag.

>Eg. `<button id="red_button" class="red" ampAction="dismissed_on_iphone" type="dismiss">some text here</button>`
Replace `some text here`

2. For the **Ok button** replace the text betewen the `<button id="black_button"></button>` tags.
>Eg. `<button id="black_button" class="black" type="submit">some text here</button>`
Replace `some text here`
---
##### If you wish your **Ok button to open up a browser** on the phone with the url of your choice you should edit the attributes within the `<form>` tag.

```<form action="http://getdrop.com?ampAction=visited_getDrop&ampExternalOpen=true">```

>`http://getdrop.com` - the url that will open in the external browser

>`?ampAction=visited_getDrop` - **visited_getDrop** is the keyword that will appear in in the Events Dashboard of localytics.  You may change that keyword to an event keyword of your choice.

>`&ampExternalOpen=true` - this must be set to allow the external browser to open. 
___

### To include your own image

Once you have finished editing this file, you should include an image within the template by deleting the current image and adding a new image of your choice named **sampleImage.png**

### To test what your changes look like

- Open the file index.html in Chrome Browser. 
- Right-Click and select 'Inspect Element'
- Set the device to either 'iPhone' or 'iPad' and the orientation to 'landscape'

![chrome]
[chrome]: (https://github.com/dropkitchen/inapp-msg-templates/blob/master/chrome_debug_screenshot.png)

### When you are happy with the result 
Zip the folder for upload to Localytics by selecting **all** the files included in the folder: 

1. Museo_Slab_900.otf
2. OpenSans-CondLight.ttf
3. OpenSans-Regular.ttf
4. index.html
5. localytics.css
6. sampleImage.png

**right click** and select 'Compress 6 items'.

When you have created the new archive upload the archive to the message builder according to localytics instructions [here]

#### Some Gotchas

1. Once you have uploaded the artwork to Localytics Dashboard you will have the opportunity to preview the work.  The preview is not 100% reliable, so the only reliable way to test the artwork is on an actual device
2. Currently Test Mode is not working so you must [at the moment anyway] test on a live campaign.  You should create an audience that includes only yourself so that while you are testing only you will receive the in-app message.
3. According to Localytics "With regards to the in-app timing, when choosing an "Audience" of everyone, the message will send immediately.  It can take a bit time if you are not choosing an Audience of "everyone" as we have a segmenter that has to filter through the data and pull out the particular users you are filtering for." This means that you may wait up to 30 minutes after the campaign has been scheduled to go live to see the message appear on your device.  ****NOTE *** Old messages will still appear during this time. 

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does it's job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [iphone-center-modal-template]: <https://github.com/dropkitchen/inapp-msg-templates/tree/master/iphone-center-modal-template>
   [index.html]: <https://github.com/dropkitchen/inapp-msg-templates/blob/master/iphone-center-modal-template/index.html>
   [here]: <http://docs.localytics.com/#Marketing/Messages/file-uploader.html>
   [ipad-center-modal-template]: <https://github.com/dropkitchen/inapp-msg-templates/tree/master/ipad-center-modal-template>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [marked]: <https://github.com/chjj/marked>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [keymaster.js]: <https://github.com/madrobby/keymaster>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>
   
   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]:  <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>



