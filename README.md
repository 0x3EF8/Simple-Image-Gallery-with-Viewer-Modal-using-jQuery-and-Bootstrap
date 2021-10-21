# Simple-Image-Gallery-with-Viewer-Modal-using-jQuery-and-Bootstrap

![img](./image1.png)
![img](./image2.png)

simple a Image Gallery web application with an image viewer modal.The Image Viewer will also have control button for navigating to the pervious or next image. We will be using Bootstrap for the design of the application and jQuery to dispaly image on the viewer modal and for navigation control functionalities.


# Getting Started
In this tutorial, I used Bootstrap v5 for the design of application. And, kindly download also the jQuery Library. After that, compile you CSS and Script assets into a directory.

# Creating the Custom CSS
The following code is the custom Cascading Style Sheet for the design of the gallery images, container, and viewe modal. It also includes the style for the navigator buttons (Next and Previous) of the for the Images Viewer Modal. Save this file as custom.css and In my case this was located inside the CSS directory.

css code here 

       .img-item .card 
       {
        cursor: pointer;
    }
 
    .img-item .card:hover .img-thumb {
        cursor: pointer;
        transform: scale(1.4);
        filter: brightness(1);
    }
 
    .img-container {
        width: calc(100%);
        height: 40vh;
        overflow: hidden;
    }
 
    .img-thumb {
        width: calc(100%);
        height: calc(100%);
        object-fit: scale-down;
        object-position: center center;
        transition: transform .3s ease-in;
        filter: brightness(0.8);
    }
 
    #img-viewer-container {
        height: 70vh;
        width: calc(100%);
        position: relative
    }
 
    img#img-viewer {
        height: calc(100%);
        width: calc(100%);
        object-fit: scale-down;
        object-position: center center;
    }
 
    .control-prev,
    .control-next {
        cursor: pointer;
        height: 75px;
        width: 75px;
        opacity: .3;
    }
 
    .control-prev:hover,
    .control-next:hover {
        opacity: 1;
        background-color: #00000033;
    }
 
    .control-prev {
        left: 0
    }
 
    .control-next {
        right: 0
    }
 
    .control-next-container {
        right: 0
    }
 
    .control-prev:before {
        content: "";
        height: 50px;
        border-left: 5px solid white;
        position: absolute;
        top: 47%;
        left: 2em;
        transform: rotate(-56deg);
    }
 
    .control-prev:after {
        content: "";
        height: 50px;
        border-left: 5px solid white;
        position: absolute;
        bottom: 47.8%;
        left: 2em;
        transform: rotate(56deg);
    }
 
    .control-next:before {
        content: "";
        height: 50px;
        border-left: 5px solid white;
        position: absolute;
        top: 47%;
        right: 2em;
        transform: rotate(56deg);
    }
 
    .control-next:after {
        content: "";
        height: 50px;
        border-left: 5px solid white;
        position: absolute;
        bottom: 47.8%;
        right: 2em;
        transform: rotate(-56deg);
    }
