# WaferPlayer.js

WaferPlayer.js simple video player Framework 

with wafer player.js we can make multi resolutions easily and there is also a subtitles/CC feature

![waferPlayer.js](https://github.com/Illeandra/WaferPlayer/blob/158e46a1747e56167e1d62104fb9cec1abf22177/Screenshot%202021-09-20%20194627.png)

**application :**

      new waferPlayer('#myvideo').config(
                'resolution': [
                                {
                                    'tag': 'HD', 
                                    'url': 'path/hdvideo.mp4',
                                    'as' : 'default' // optional, default is 1st
                                 },
                                 {
                                    'tag': 'FHD',
                                    'url': 'path/fhdvideo.mp4'
                                 }
                                ],
                  'subtitles': [
                                 {
                                    'tag': 'ENG',
                                    'url': 'path/subENG.vtt'
                                  },
                                  {
                                     'tag' : 'IDN',
                                     'url' : 'path/subIDN.vtt'
                                  }
                                ], 
                  'interface': {
                                 'image' : {
                                              'url': 'path/img', 
                                              'position': 'top-left'
                                            },
                                  'color' : '#2A4DF9', // default #FF4949
                                  'autohide' : '6' // insecond, default is 5 
                                  });
             
***
                     
## Explanation

.config accepts JSON input with keys resolution, subtitles and interface


> ### resolution
>
> resolution accepts array containing JSON with keys tag and url

> > tag contains the code or type that will be seen by the user
> > 
> > _example : HD, FHD or 4K and other_
> > 
> > url is video path
> > 
> > _example : localhost/video/fullHDvideo.mp4_
***
> ### subtitles
>
> subtitles accepts array containing JSON with keys tag and url

> > tag contains the code or type that will be seen by the user 
> >
> > _example : ENG, IDN or RUS and other_
> > 
> > 
> > url is subtitle vtt file path 
> > 
> > _example : localhost/subtitle/subtitleENG.vtt_
***
> ### interface
>
> interface accepts JSON with keys image, color and autohide

> > image accepts JSON with keys url and position
> > 
> > url is image file path
> > _example : localhost/imagePath/image.img_
> > 
> > position is image position available value 
> > 
> > * top-left
> > * top-right
> > * bottom-left
> > * bottom-right
> > 
> > if position not set the image will be in the center of the video player
     
> **color is video player interface color**
  
> **autohide is time to hide control bar video player**
