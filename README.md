A collection of HeSuVi 7.1 impulse responses that i've recorded and edited.

_Note: all recorded at 48Khz. For 44.1Khz, I recommend you use the resample script in https://github.com/ThreeDeeJay/HRIR-Batch-Converters or open them in Audacity and re-save._

Files:

## Apple Spatial
### Generic
**AppleSpatial** - Apple's "Spatial Audio" renderer used by AirPods with Apple Devices. A fairly uncolored HRIR with minimal reverb, great clarity, and a high degree of openness. Rendered in Logic Pro with the 
**AppleSpatialMovie** - The variation of Apple's renderer that is seen on Apple TV. This version includes more reverb and bass boost. Recorded in Logic Pro with the "Movie" renderer mode.

### Personalized
**ApplePersonal** - Same as above, but with AirPods connected and the personalized profile option enabled in Logic Pro.  
**ApplePersonalMovie** -  Same as above, but with AirPods connected and the personalized profile option enabled in Logic Pro.

### Apple Speaker Spatial (Crosstalk Cancellation)
**AppleSpatialSpeakerT** - Apple's crosstalk cancellation implementation as seen in their devices, active when you play spatial content through speakers. This is the profile for the Mac speakers. This has one of the best directionality effect that i've found when testing with desktop speakers, but the tonality is obviously tuned for a laptop. May try to fix with EQ down the line. (T -  Trimmed excess from the end)
**AppleSpatialSpeakerTB** - Same as before, but trimmed from the beginning as well for latency purposes. This may result in slight artifacting, hence why it didn't replace the former version.

## Dolby Renderer
### Generic
_Coming soon. I've recorded them, just have not gotten around to editing._

### Personalized
**AtmosRenderer-Far-Personalized** - Dolby's "Atmos Renderer" with a personalized profile applied, taken with the "far" preset. This introduces strong room acoustics and reflections, just like Apple's Movie spatial audio.  
**AtmosRenderer-Mid-Personalized** - Dolby's "Atmos Renderer" with a personalized profile applied, taken with the "medium" preset. This is fairly light in reflections with practically no room simulation/acoustics, similar to Apple's standard spatial audio.  
**AtmosRenderer-Near-Personalized** - Dolby's "Atmos Renderer" with a personalized profile applied, taken with the "near" preset. This has practically no reverb or room acoustics, making it a bit flat, but not as "strong" as the other presets.  

### Trimmed:
**AtmosRendererT-Far-Personalized** - Same as before, trimmed the excess of the end for CPU usage.  
AtmosRendererT-Mid-Personalized  
AtmosRendererT-Near-Personalized  

**AtmosRendererTB-Far-Personalized** - Same as before, but also trimmed off of the beginning for latency purposes.  
AtmosRendererTB-Mid-Personalized  
AtmosRendererTB-Near-Personalized  
