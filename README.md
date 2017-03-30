# Polymer element for ImageEngine

[https://www.scientiamobile.com/page/imageengine] ImageEngine

ImageEngine is an intelligent image CDN for optimizing, compressing and resizing images. ImageEngine will enhance your responsive images by enabling support for HTTP2, automatic webp conversion, Client Hints and more.

It is likely that ImageEngine will shave off 50-60% of data traffic generated by images on your site. To better support mobile devices, ImageEngine relies on WURFL for server side device detection in cases where responsive images and Client Hints fall short.

Registration is required to get the most out of ImageEngine. 

Images weight is by far the most important challenge to address when optimizing a web page for the plethora of devices on the web today. This is why ImageEngine will instantly give your users a better experience by reducing load time of your page. Not to mention the reduced data cost.

ImageEngine works as a CDN proxy. By referencing the ImageEngine servers and providing the full URL to the original image as a parameter, ImageEngine will identify the device, and its capabilities, and resize and optimize the image accordingly.

Client Hints

The plugin will enable Client Hint support for your site. Client Hints, with information about the viewport size, device pixel ratio and actual image size, are added to the image request (HTTP header) enabling ImageEngine to resize the image with surgical precision.

HTTP2 support

HTTP will give additional performance improvement on the network level. ImageEngine supports HTTP2 over SSL, which means that if you serve your sites and images by https://, ImageEngine will automatically serve all images over HTTP2.

WebP

WebP is a lightweigh image format with great quality. WebP is well supported by browsers. ImageEngine will detect if the end user's browser supports WebP and automatically convert any format to WebP to increase performance.

## Using image-engine in your polymer project


1. `bower install imageengine-polymer  --save`
   * `After installation as one time configuration you have to go to bower_componentsimageengine-polymer/image-engine.html` and replace token value from "try" to your token value.
   * Go to [https://www.scientiamobile.com/page/imageengine](https://www.scientiamobile.com/page/imageengine) to know more about getting your own ImageEngine token.

2. import `path_to_your_bower_components/imageengine-polymer/image-engine.html`

3. use element as `<imageengine-polymer imagesrc="https://yourhostedimage.jpg" https=true width="" height="" ></imageengine-polymer>`
     * note that if your image(s) use https , make sure you set https=true param while calling the element,if you are not using height and width options of ImageEngine assign them to an empty string (image(s) will take default width and height).

     * imagesrc is a mandatory param/property for this polymer element .




## Running the demo


1.  Download and install Node from [https://nodejs.org/](https://nodejs.org/). Node includes the node package manager command, `npm`.

2.  Install `bower` and `polyserve`:

        npm install -g bower polyserve

3.  Clone this repo:

        https://github.com/WURFL/ImageEngine-polymer-element.git
        
4.  Change directory to your local repo and install dependencies with `bower`:

        cd ImageEngine-polymer-element
        bower install
        
5.  To preview your element, run `polyserve` from the repo directory:

        polyserve
        
    Open `localhost:8080/components/image-engine/demo/` in your browser. (Note that the path uses `image-engine`—the 
    component name listed in this element's `bower.json` file—rather than the actual directory name.) 
    

