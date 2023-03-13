# espHome_media_volume_remote

First, put blueprint-2nd-snesor.yaml into /config/blueprints
2 Set up input_number helper with the name ' target ' (optional use 'average sensor' for remote sensor!)
3 Make automation from blueprint, name does not matter.
4 Change substutions in esp_volume_remote.yaml
5 on espHome click create new, name it esp_volume_remote, flash and adopt(save the keys and board type etc, put those in esp_volume_remote.yaml)
6 edit new espHome node, copy and paste edited esp_volume_remote.yaml indo congfig
7 add devide to home assistant
Enjoy!

Control Media entity volume with a display showing the volume level, artist and title on screen. Neopixel ring Volume level feedback.
#######################################################
#       Click=Next Page - Double click=SKIP/NEXT      #
#     Short Hold <2s=Mute - Hold >2s=Toggle Screen    #
#######################################################
- Clockwise = Volume +   
- Anti-Clockwise = Volume - 

Display text is shown if available form media_payer2
Media3 is for the 3rd page media player (has to be same entity for audio and video )
Other version-
[Display only no LEDs - esp_volume_remote(Display Only).yaml]

![image](https://github.com/kiasarecool/espHome_media_volume_remote/blob/main/pics/1.jpg)
![image](https://github.com/kiasarecool/espHome_media_volume_remote/blob/main/pics/2.jpg)
![image](https://github.com/kiasarecool/espHome_media_volume_remote/blob/main/pics/3.jpg)

Parts:

5V Individual Addressable RGB LED NeoPixel Ring For ArduinoWS2812- 12 LED ( aliexpress, $0.77 ea + shipping )
https://www.aliexpress.us/item/3256804900290133.html?spm=a2g0o.order_list.order_list_main.10.54f61802sL1qIr

rotary encoder with push/click (aliexpress $0.56 + shipping )
https://www.aliexpress.us/item/3256802644265906.html?spm=a2g0o.productlist.main.5.6bfa54c4ycTVu0&algo_pvid=7f264cee-db4a-4a9b-a675-d65e911d5ad2

D1 mini esp32 s2 ( aliexpress $2.45 + shipping )
https://www.aliexpress.us/item/3256805048425363.html?spm=a2g0o.productlist.main.23.1e344136EfEIH2&algo_pvid=5076a01a-4648-47da-8e3b-78ed1f16e699

1.5" RGB oled 128x128 ( amazon prime $18.59 )
https://www.amazon.com/gp/product/B07D9NVJPZ/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1

3D printed box
STL provided
 
You will also want (or you're gonna be soldering!)
Female to female jumper wires
AND
make 2 'Y' jumpers to feed an extra 3.3v and an extra ground to the componets. (all female ends)
