# streaming

## hardware setup


I realized that my photo camera can also record videos. Since then, I always use it for this purpose.

- I have a Nikon D850, but any other decent photo camera works just as well as a webcam.
- The camera is mounted on a tripod.
- It is connected to a power outlet because otherwise, the battery would need to be replaced every few hours during video recordings.

### HDMI Capturing

- Theoretically, you could simply connect the camera to the computer via USB – in my case, with the Nikon Webcam Utility. However, it was limited back then (it only worked in Zoom but not in Teams or WebEx).
- This was frustrating for me.
- Instead, I got a mini HDMI 4-channel mixer, the [Atem Mini](https://www.blackmagicdesign.com/at/products/atemmini). It has additional advantages, for example, I can also mix the iPad or screen content with the green screen, and always be seen in the foreground in front of the PPT or coding window.
- The green screen is from [Elgato](https://www.elgato.com/de/green-screen) (you didn't see it in use yesterday).

### Audio

- Good audio is important – and as long as you don't want to combine it with good video simultaneously, it's super easy. I use a [Blue Yeti microphone](https://www.bluemic.com/de-de/products/yeti/), which can be easily connected via USB – done. And it's dramatically better.
- Unfortunately, I have problems with the audio input on the ATEM Mini and therefore route audio and video separately (resulting in a few frames delay). Did you notice this yesterday?
- Nowadays I sue the yeti for most teams/zoom calls and it works great. But for recordings and live streams I use https://rode.com/de/microphones/wireless/wirelesspro directly connected timecoded to my camera for the best streaming/recording/audio experience
- AH CQ18T
- shure sm7db
- audio playback
 - https://github.com/freeman-jiang/beatsync

### video

- d850
- secondary camera
- teleprompter

### Lighting

- Instead of investing in an extremely expensive camera, good audio and lighting are better investments.
- I use:
  - 2x Key Lights from [Elgato](https://www.elgato.com/de/key-light) – they are great and you can adjust the brightness and color temperature.
  - A smart lamp from [Luke Roberts](https://www.luke-roberts.com/products/smart-lamp-model-f-white?ls=de) with a slight blue/purple tint for the background, or additional white lighting when using the green screen.

### Control

- With the [Stream Deck](https://www.elgato.com/de/stream-deck-mk2) you can flexibly control the lights, the HDMI mixer (ATEM), or any other actions with a hardware button and even record and play macros.
- One or two USB hubs.
- Lots of cables (HDMI, USB, etc.).
- For controlling the Atem Mini: a small network switch and cables (only works via TCP-IP).

### On-Screen

- The [Logitech Spotlight Presentation Remote](https://www.logitech.com/de-at/products/presenters/spotlight-presentation-remote.910-004862.html?crid=11) is a great laser pointer that also works remotely in Webex or for 1000 people with 3 projectors simultaneously – because it's digital. The magnifier and focus gimmicks are great!
- [DemoPro](http://www.demoproapp.com/) (Mac) offers similar features for Windows for countdown timers and drawing directly on the screen and is a good addition.

I hope you find some useful tips here.


### atem mini tricks

- ISO davinci resolve integration
  - https://www.youtube.com/watch?v=YtsVUtm9jmE
  - 4k https://www.youtube.com/watch?v=CZpcvqOPAKo
  - replay
    - https://www.youtube.com/watch?v=aMxg4ECnyms
    - https://www.youtube.com/watch?v=FcDULDr3QQM
- resolve tricks
  - https://www.sideshowfx.net/davinci-resolve-color-panel-stream-deck-plus-mac?aff=7 https://jonnyelwyn.co.uk/film-and-video-editing/controlling-davinci-resolve-with-the-stream-deck/
- remote guest atem
  - https://www.youtube.com/watch?v=fKpusuY-cjs
- macros
  - https://www.youtube.com/watch?v=BegP_UWs454

## paid
- https://streamyard.com/
- https://www.ecamm.com/

## opensource
- https://obsproject.com/de
  - https://vdo.ninja/
    - https://docs.vdo.ninja/advanced-settings/setup-parameters/and-sink
    - https://docs.vdo.ninja/advanced-settings/setup-parameters/and-audiooutput
    - !!! https://github.com/steveseguin/electroncapture !!!
    - Quality https://docs.vdo.ninja/getting-started/even-higher-quality-video
  - https://support.volume.com/hc/en-us/articles/4425732789911-Feature-Live-Guests-with-VDO-Ninja-OBS

### obs plugins

- https://obsproject.com/forum/resources/obs-shaderfilter.1736/
- https://obsproject.com/forum/resources/advanced-masks.1856/
- https://obsproject.com/forum/resources/stroke-glow-shadow.1800/
- https://obsproject.com/forum/resources/composite-blur.1780/
- https://obsproject.com/forum/resources/3d-effect.1692/
- https://obsproject.com/forum/resources/downstream-keyer.1254/
- https://obsproject.com/forum/resources/source-clone.1632/
- https://obsproject.com/forum/resources/move.913/
- audio mixer
  - https://www.voxengo.com/product/marvelgeq/
- https://obsproject.com/forum/resources/source-record.1285/
- https://obsproject.com/forum/resources/aitum-vertical.1715/ vertical
- https://streamer.bot/features
- combined sourc switcher https://obsproject.com/forum/resources/source-switcher.941/ with move transition https://github.com/exeldro/obs-move-transition

## AI video summarization

- https://klap.app/

## AI video generation

- https://www.heygen.com/
- https://lumalabs.ai/dream-machine
- https://app.runwayml.com/login gen-3
- https://invideo.io/
- https://www.revid.ai/

## transcription & captions

- https://sonix.ai/de
- https://www.heygen.com/

## multi streaming

- https://www.boxcast.com/
- https://restream.io

## streaming server

- https://owncast.online/


## zoom tips

- https://www.youtube.com/watch?v=I473FLo-Bug
- https://www.youtube.com/watch?v=aK4S4wrmhF4&t=531s

## ppt tips

- wow indeed https://discussions.apple.com/thread/7179965?sortBy=rank open PPT in non full screen mode makes it work

## scene switching

### super source

- great makros https://www.a2z-productions.com/atem-resources
- visual builder and buy of macros https://layouts.heretorecord.com/

## streaming utilities

- https://heretorecord.gitbook.io/h2r-graphics
- stingers https://stingers.heretorecord.com/


## vst plugins

### quality

- https://www.accentize.com/dxrevive/

## stock content

### audio

- https://artlist.io/

### visual

- https://pixabay.com/de/
