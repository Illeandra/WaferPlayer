# WaferPlayer.js
WaferPlayer.js simple video player Framework 

with wafer player.js we can make multi resolutions easily and there is also a subtitles/CC feature

application :

new waferPlayer('#myvideo').config('resolution': [{
                                                     'tag': 'HD', 
                                                     'url': 'path/hdvideo.mp4',
                                                     'as' : 'default' // optional, default is 1st
                                                   },
                                                   {
                                                     'tag': 'FHD',
                                                     'url': 'path/fhdvideo.mp4'
                                                   }
                                                   ],
                                   'subtitles': [{
                                                   'tag': 'ENG',
                                                   'url': 'path/subENG.vtt'
                                                 },
                                                 {
                                                   'tag' : 'IDN',
                                                  'url' : 'path/subIDN.vtt'
                                                 }], 
                                   'interface': {
                                                  'image' : {
                                                             'url': 'path/img', 
                                                             'position': 'top-left'
                                                             },
                                                  'color' : '#2A4DF9', // default #FF4949
                                                  'autohide' : '6' // insecond, default is 5 
                                                 }
                                   );
