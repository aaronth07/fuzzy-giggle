A collection of HeSuVi 7.1 impulse responses that i've recorded and edited.

_Note: all recorded at 48Khz. For 44.1Khz, I recommend you use the resample script in https://github.com/ThreeDeeJay/HRIR-Batch-Converters or open them in Audacity and re-save._

# Impulse Responses:

## Apple Spatial  
### Generic  
**AppleSpatial** - Apple's "Spatial Audio" renderer used by AirPods with Apple Devices. A fairly uncolored HRIR with minimal reverb, great clarity, and a high degree of openness, but with a very close rendering distance. Rendered in Logic Pro with the "Music" renderer mode.  
**AppleSpatialMovie** - The variation of Apple's renderer that is seen on Apple TV. This version includes more reverb and bass boost. Recorded in Logic Pro with the "Movie" renderer mode.  

### Personalized    
**ApplePersonal** - Same as above, but with AirPods connected and the personalized profile option enabled in Logic Pro.  
**ApplePersonalMovie** -  Same as above, but with AirPods connected and the personalized profile option enabled in Logic Pro.  

_Edited versions:_
**ApplePersonal+** - Same as ApplePersonal, but with the reverb and non-direct sound boosted in magnitude after about 7ms and onward. Tonality should be very similar so no graphs.  
**ApplePersonal-DeVerb** - Exact opposite of the "+" version, with reverb after a certain point cut with smooth fade off. I can't remember specifics on time but I believe it was about 12-15ms that I started fading out, please correct me if you open the waveform.

At this time I do not plan on making non-personalized edited versions, apologies. Perhaps someday if I have the free time. I will say that Apple's personalization effect is not very extreme (right in the middle), so even the personlized versions should still be usable for the vast majority 

### Apple Speaker Spatial (Crosstalk Cancellation)  
**AppleSpatialSpeakerT** - Apple's crosstalk cancellation implementation as seen in their devices, active when you play spatial content through speakers. This is the profile for the Mac speakers. This has one of the best directionality effect that i've found when testing with desktop speakers, but the tonality is obviously tuned for a laptop. May try to fix with EQ down the line. (T -  Trimmed excess from the end)  
**AppleSpatialSpeakerTB** - Same as before, but trimmed from the beginning as well for latency purposes. This may result in slight artifacting, hence why it didn't replace the former version.  

_Note: Apple's profiles were directly rendered in Logic Pro from the original 7.1 impulse response testing file, negating the need for manual trimming or trimmed versions._

## Dolby Renderer  
### Generic  
**AtmosRenderer-Far-Generic** - Dolby's "Atmos Renderer" without a personalized profile applied (default generic), taken with the "far" preset. This introduces strong room acoustics and reflections, just like Apple's Movie spatial audio.  
**AtmosRenderer-Mid-Generic** - Dolby's "Atmos Renderer" with a personalized profile applied, taken with the "medium" preset. This is fairly light in reflections with practically no room simulation/acoustics, similar to Apple's standard spatial audio.  
**AtmosRenderer-Near-Generic** - Dolby's "Atmos Renderer" with a personalized profile applied, taken with the "near" preset. This has practically no reverb or room acoustics, making it a bit flat, but not as "strong" as the other presets.  

_Note: The generic versions of the Dolby Profile are already trimmed in both ends._

**AtmosRendererFar-EQComp-V1.txt** - Rough EQ to correct the Atmos Far Renderer's odd tonality, for the purpose of getting the wider/expanded space, room reflections, and reverb without the wonky tonality changes/speaker emulation. V1 to specify that it is rough and not perfect. Works with both generic and personalized.

### Personalized
**AtmosRenderer-Far-Personalized** - Dolby's "Atmos Renderer" with the "far" preset, with a personalized profile applied. Personalization was captured with the Dolby PHRTF app and uploaded to the renderer. I find that the effect of personalization is very minimal in comparison to Apple's Spatial or an actual HRTF recording.  
**AtmosRenderer-Mid-Personalized** - Same as above, but taken with the "medium" preset.  
**AtmosRenderer-Near-Personalized** - Same as above, but taken with the "near" preset.  

_Note: Scans were done with the Dolby PHRTF	app beta testflight. A newer/white labeled version of this app can be used with the SoundID Tools app, of which I am unsure if there are any improvements to the scanning accuracy or model itself._

### Trimmed:
**AtmosRendererT-Far-Personalized** - Same as before, trimmed the excess of the end for CPU usage.  
AtmosRendererT-Mid-Personalized  
AtmosRendererT-Near-Personalized  

**AtmosRendererTB-Far-Personalized** - Same as before, but also trimmed the beginning for latency purposes. 
AtmosRendererTB-Mid-Personalized  
AtmosRendererTB-Near-Personalized  

# Plots
Out of curiousity, and to attempt to match/map both an HRTF preference curve and to compensate some of the wonky tonality, I have also recorded sweeps and graphed them using REW. Sweeps were recorded at 24/48 with the edited HeSuVi BRIR applied from the left ear. I found that it was best to re-record a sweep and graph it rather than attempting to plot the binaural impulse response directly. Everything was done with REW, psychoacoustic smoothing, matched at 630Hz 2/oct. 

"ApplePersonal" is the personalized profile, while "AppleSpatial" is the non-personalized.

<img width="2121" height="1063" alt="AppleSpatial_cae" src="https://github.com/user-attachments/assets/2870aad2-524e-4ee5-92d6-3ba755b88e06" />
<img width="2121" height="1063" alt="ApplePersonal_cae" src="https://github.com/user-attachments/assets/1e926ee6-642b-4573-aa4f-2d42230b46ca" />
<img width="2121" height="1063" alt="AppleSpatialMovie_cae" src="https://github.com/user-attachments/assets/2fa360f6-960f-4b28-8391-948e08adf107" />
<img width="2121" height="1063" alt="ApplePersonalMovie_cae" src="https://github.com/user-attachments/assets/8d1f6d0c-ba2e-4759-8fc2-1765fe8168df" />
<img width="2121" height="1063" alt="AtmosRendererNearGeneric_cae" src="https://github.com/user-attachments/assets/471f907f-b6c9-4f49-9752-bf30d81ab051" />
<img width="2121" height="1063" alt="AtmosRendererNearPersonalized_cae" src="https://github.com/user-attachments/assets/7118d2f8-e3b2-4ed8-9b7a-9967b1a66306" />
<img width="2121" height="1063" alt="AtmosRendererMidGeneric_cae" src="https://github.com/user-attachments/assets/d342e7b5-89b0-4c80-b54a-c69771a7a73f" />
<img width="2121" height="1063" alt="AtmosRendererMidPersonalized_cae" src="https://github.com/user-attachments/assets/6f252782-2157-4a14-b7b3-e2de63cd6733" />
<img width="2121" height="1063" alt="AtmosRendererNearGeneric_cae" src="https://github.com/user-attachments/assets/af6cc746-8631-4384-89cc-468e766f5cdb" />
_Possibly mislabeled_
<img width="2121" height="1063" alt="AtmosRendererFarPersonalized_cae" src="https://github.com/user-attachments/assets/e09d98e4-41ce-403e-ab9e-8c9f1b46d1e4" />

Results are... interesting. I'm still not sure what the best way to capture digital impulse responses/sweeps are since I believe this was still subject to interference/jitter, and I didn't find the results to be very useful enough to begin compensation for some of the more extreme charactaristics of the responses (e.g. Apple Spatial Movie's bass). I may try to rerecord the sweeps with a different device, or render them in a DAW to see if I can achieve better results. 
