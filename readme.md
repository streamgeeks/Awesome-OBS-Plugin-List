# PLUGIN TO THE PLUGINS


The core OBS Studio application features a robust API that developers use to create plugins to extend the functionality of OBS. Plugins can be found to do everything from instant replay to automatic scene switching making OBS as powerful as many paid video production software suites. Plugins for OBS can be found in the resources section of the [OBS Forum page](https://obsproject.com/forum/resources/). In order to download a plug-in you will generally be directed to GitHub because all OBS plugins must be open source. Github is a social source code sharing website that allows software developers to interact and share their work. By default, OBS plugins on the website are sorted by their last update. You may find it more useful to filter the 120+ OBS Studio plugins by “most downloaded” or “best rated” to find the most reliable and useful plugins. 
 
<h2 align = "center" ><img src="/img1.png" ><h2>
<h4 align = "center"><b>OBS Plugins can be sorted with Filters in the Forums page.</b></h4>

After sorting through dozens of OBS Studio plugins, the following list has been compiled of the top plugins for OBS. Each plugin in this list will be reviewed in greater detail in an upcoming chapter. 

- Plugins for Production  :movie_camera:
    - [**Multiple RTMP Output**](#multiple-rtmp-streaming-destinations) - This plugin allows you to stream to multiple CDNs at the same time via RTMP. This is popular for live streaming to YouTube and Facebook at the same time for example but does require extra upload bandwidth to work properly. 
    - [**Advanced Scene Switching**](#advanced-scene-switcher-plugin) - This plugin is designed to automatically switch between OBS scenes based on a variety of triggers such as audio, media, and hotkeys. It can be used to switch to a specific camera for example, when a microphone becomes active. 
    - [**Source Docks**](#source-dock-plugin) - This plugin allows you to dock any source inside the OBS interface. This is a great way to quickly view and control media inside of the OBS interface. 
    - [**Source Record**](#source-record-plugin) - This plugin creates a filter you can use to record a specific source independently from the main video recording. 
    - [**Replay Source**](#replay-source) - This plugin allows you to create live instant replays using OBS. It allows you to apply a filter to any given source which will record the video for instant playback in your computer memory. This plugin offers the ability to use hotkeys and play video back in slow motion. This is a great plug-in for sports productions. 
    - [**NewTek NDI® Integration**]() - This plugin allows you to connect OBS to NDI® video sources in a couple different ways. First you can bring NDI® video sources on your network into OBS by adding NDI® as a source. Additionally you can output video from your OBS production as an NDI® source on your network. And finally, you can add an NDI® output filter on any source. This allows you to output individual sources as NDI® outputs on your network (more on NDI® in an upcoming chapter).
- Plugins for Audio :headphones:
    - [**OBS Music Edition**]() - This is a custom build of OBS which is designed for audio producers. This build of OBS is compatible with VST3 plugins which are used by top music producers around the world. 
    - [**Audio Monitor**](#audio-monitor-plugin) - This plugin allows you to use a filter to route audio to any virtual or physical audio output available on your computer. This is often used to send an audio output from OBS to software such as Zoom. 
    - [**VST2 Plugins**]() - There are a variety of free VST2 plugins available from companies such as Reaper.fm that you can use with OBS. The Reaper.fm VST2 plugins work very well with OBS and will be covered in an upcoming chapter. 
- Plugins for Control :arrow_forward:
    - [**Websockets**]() - The OBS Websockets plugin created an API you can use to remotely control OBS. There are many plugins available that use this API and OBS Remote will be one that is reviewed in this book.
    - [**Filter Hotkeys**](#filter-hotkeys) - This plugin allows you to use hotkeys to turn filters on and off. This is ideal for toggling effects on and off during a production. 
    - [**PTZ Controls**]() - PTZ camera controls are available to operate PTZ cameras from the OBS interface. This is ideal if you have PTZ cameras that you are working with inside of OBS.
    - [**Virtual Audio Cables**](#working-with-virtual-audio-cables) - While these are not officially a plugin, they will enable you to use OBS in new and powerful ways. Virtual Audio Cables are technically audio drivers which can be used to route audio on your computer using OBS.
- Plugins for Graphics :computer:
    - [**Animated Lower Thirds**](#animated-lower-thirds) - This plugin allows you to control animated lower thirds with a dockable controller. The dockable controller is well designed for managing lower third content and the animations used.
    - [**Move Transitions**]() - This plugin allows you to control transitions for individual sources as they move with scene transitions. Therefore, individual sources can move in and out of scenes with custom effects as you switch between scenes.
    - [**Closed Captions**](#closed-captions-for-obs) - While this is not technically a plug-in, Web-Captioner is one of the best tools for closed captions. Web-Captioner takes an audio output from OBS and creates an HTML web-page that can be brought back into OBS with the closed captions. 
    - [**Background Removal**](#background-removal) - This plugin uses an advanced neural network to remove the background of images and video sources. This allows you to apply an audio/video filter to any image or video and replace the background with something else. This is popular for green screen applications used to create virtual sets or blurred backgrounds. 
    - [**OBS Color Monitor**]() - This plugin adds crucial tools for color grading which include a vectorscope, a waveform and a histogram. These tools allow you to properly color balance live video sources. A vectorscope is a visual representation of color in a live video source. A waveform monitor is considered the counterpart to the vectorscope and it handles exposure and brightness. The histogram displays red, green and blue colors for the select source on a graph.

Each of these plugins will help you gain new capabilities inside of OBS. The process of installing a plugin into OBS is very straightforward. All you need to do is copy and paste the plug-in files that you download directly into the plugins folder for OBS on your computer. The OBS plugin folders can be found in the locations below.

## Windows:

32-bit plugins folder = ``C:\Program Files (x86)\OBS\plugins`` <br>
64-bit plugins folder = ``C:\Program Files\OBS\plugins``

## Mac:

``Applications/OBS.app/Contents/Plugins``

Here are the steps you can follow to install any OBS plugin.

1.	Download the plugin files from GitHub
2.	Unzip the files on to your computer 
3.	Copy and paste them into the OBS plugins folder
4.	Launch the OBS application

Once you have completed the steps above, the plugin you have installed should become available inside of OBS. It’s really that simple. Some plugins make installation even simpler with an installation wizard that handles this process for you. The following chapters will outline each plug-in on the list and the capabilities they add to OBS. You can pick and choose which plugins will add value to your production and watch the online tutorial videos available in the Udemy course with this book to see how they work. In some cases, plugins can be used together to create new functionality the developers didn’t intentionally plan out. So enjoy each plug-in overview and keep an open mind to the abilities each adds while you think about the overall functionality of OBS.

### Key Takeaways:

1.	Hundreds of developers have created plugins for OBS that extend the functionality of the software. 
2.	OBS plugins are easily to install manually and some developers even include auto-installation wizards to make the process easier.
3.	All OBS plugins are open source and can therefore be customized to fit your needs.
4.	This book includes reviews for a long list of reliable plugins that can significantly increase the capabilities of OBS for your video productions. 



## MULTIPLE RTMP STREAMING DESTINATIONS

As content creators seek to grow their audiences and reach new people, many want to begin streaming to multiple platforms. For example, streamers with channels on YouTube may want to expand their audience to Facebook. Gamers streaming to Twitch may also like the stream to be available on YouTube. In the past, OBS users were limited to streaming to one platform. To send streams to multiple places, many users had to change to different production software or use a third-party service to restream the OBS output to multiple platforms. While restreaming with cloud-based streaming providers is a great way to reduce computer processing and upload bandwidth requirements, many OBS users have computers and internet speeds that can handle streaming to multiple destinations simultaneously. The Multiple RTMP streaming plugin makes it possible to stream to as many destinations as your computer and internet connection can handle.

<h2 align = "center" ><img src="/img2.png" ><h2>
<h4 align = "center"><b>Multiple RTMP Output is easily configured using standard RTMP server and key information.</b></h4>


**Installing Multiple RTMP Output**
The Multiple RTMP Output plug-in is available for Mac and PC and can be downloaded from the OBS website https://obsproject.com/forum/resources/multiple-rtmp-outputs-plugin.964/. Self installation wizards are available for the Mac and Windows PC versions. This is the best route for most users. If you would like to install the plug-in manually, extract the .zip file and place the plug-in files in the correct folder on your computer. When you are done, restart OBS. 

**Using Multiple RTMP Output**
If the plug-in is installed correctly, you should see it as a floating panel in the upper left corner. This is a dockable panel, so you can move it around and place it anywhere in the OBS user interface.

1. If it is not already configured, set up your primary stream as usual. You can access the primary stream configuration in the Settings menu in the Stream tab and more advanced options in the Output tab.
2. Go to the Multiple RTMP Output Panel and click Add New Target.
3. Manually enter the RTMP Server and RTMP Key
4. Under Video Settings, it is recommended that you leave all settings as "Get from OBS." This will enable Multiple RTMP Output to use the main OBS output and stream it to the additional server. There may be occasions when you want to use a separate encoder and settings, but know that it will significantly increase the demand on your computer's CPU. See more below under Bandwidth and CPU Concerns.
5. Under Audio Settings, it is again recommended that you use the “Get from OBS” option. But, again, you do have the option to use a separate audio source. This could be ideal for sending out a stream in another language for example. 
6. Under Other Settings, click Sync start with OBS if you want the second stream to start automatically with your primary stream.
7. Repeat this process to add any additional RTMP outputs.

**Bandwidth and CPU Concerns**
Before sharing your first stream to multiple platforms, you will want to pay attention to the use of bandwidth and your computer's CPU. First of all, even though Multiple RTMP Output can use the primary output of OBS, it will still be using up additional bandwidth in order to stream to multiple platforms. Therefore, adding just one additional target will nearly double the bandwidth used. This is an especially important consideration if you have limited upstream bandwidth. 

Try running a bandwidth test to get an idea of your available upload and download speeds. You can do this quickly by Googling “speed test” and following the instructions from Google. As a general rule, your upload bandwidth should be roughly double your total bitrate for all your streams. So, if you have an upload bandwidth of 10 Mbps, you would not want to send more than 5 Mbps. So, for example, if your primary stream is 2500 Kbps, a second stream would double that, giving you 5000 Kbps which is equal to 5Mbps. 

Adding another target could take your bandwidth use past the guideline of half your upstream bandwidth. While it is possible to get away with using more than half the upstream bandwidth, you will want to do extensive testing to be sure there aren't any problems. You can monitor your bandwidth usage using your computer’s monitoring application such as Task Manager on Windows.

As covered in the setup instructions, it is recommended that you set the video settings of your secondary sources to "Get from OBS." This takes advantage of Multiple RTMP Output's ability to share the encoding work with the primary OBS output. This saves your computer from all the extra strain of encoding multiple streams. If you do opt to encode a second stream separately, know that this will significantly impact your CPU. Adding a third source will add even more to your computer's load. Whatever settings you choose, just be sure that your PC or Mac can handle the extra work without dropping frames or crashing. This is where you can monitor your computer's performance while streaming using the OBS stats. 

#### How Multiple RTMP Output is Being Used

**Houses of Worship**
Many houses of worship are using live streaming to reach a larger audience. Some may have started streaming on YouTube and now want to expand to Facebook live or vice versa. Houses of worship often run on minimal technology budgets, so purchasing new software or using a third-party service might be out of the question. Now they can use Multiple RTMP Output right inside OBS.

**Gaming**
Gamers are using Multiple RTMP Output to stream their gameplay and commentary to multiple gaming and social media sites. Gamers with the proper hardware can even take advantage of the option to use multiple encoders. This way, they can send videos with different bitrates and resolutions to match the streaming platform.

**Pros and Cons**
Pros: It’s Free and easy to setup. It can eliminate the need for a third-party restreaming services. It does not require excessive CPU power when correctly configured.
Cons: It can push the limits of upstream bandwidth when sending multiple streams. It can be highly demanding on CPU when using separate encoders for each stream.

**Alternatives to Multiple RTMP Output** 
Currently, the only other options for streaming to multiple servers from OBS are third-party services like Castr or Restream.

**Key Takeaways**
1.	The Multiple RTMP plug-in for OBS adds important functionality. 
2.	Before this plug-in, OBS users have had to rely on third-party services to capture their stream and restream it to other sites. 
3.	Now users can stream to multiple live streaming servers without ever leaving OBS.





## ADVANCED SCENE SWITCHER PLUGIN

Many OBS users handle all the aspects of video production by themselves. In these cases, there is no dedicated producer or engineer. Instead, the streaming host is also the producer, director, camera operator, and technical director. Thanks to the flexibility and customization possibilities of OBS Studio, the software works great for solo operators who learn how to use hotkeys and controllers such as the Elgato StreamDeck. However, it still doesn't hurt to have some help keeping everything running. Advanced Scene Switcher adds switching automation to OBS with a powerful plug-in that features a bunch of options to help producers automate scene switching. 

Installing Advanced Scene Switcher
You can install Advanced Scene Switcher in the same manner as most other OBS plug-ins. It is available for download on the OBS website https://obsproject.com/forum/resources/advanced-scene-switcher.395/  For this plug-in, you will download one .zip file. When you extract it, you will see the auto-installers and files for Mac, PC, and Linux. Use of the auto-installer is recommended unless you have experience adding plug-ins manually.


<h2 align = "center" ><img src="/img3.png" ><h2>
<h4 align = "center"><b>Advanced Scene Switcher opens into a management window.</b></h4>



**Using Advanced Scene Switcher**
After installation is complete, relaunch OBS. You can access Advanced Scene Switcher in the Tools menu. Be careful not to inadvertently select Automatic Scene Switcher. The Advanced Scene Switcher dialog box can be a bit overwhelming at first. Fortunately, you won't likely need more than a couple of those tabs. However, a look through them will introduce you to the possibilities of Advanced Scene Switcher.

In the General tab, you will find some of the global settings you may need to revisit once you get some automations set up. One thing to note here is the Status section, where you can choose to automatically start the switcher when you start recording, streaming, or both. There is also an option to start the switcher on startup if it was running previously.

The rest of the tabs cover all the possible ways to use Advanced Scene Switcher. As you review the options available on each tab, notice that they all work on the same basic concepts – triggers and actions. Setting up automated scene switching is about assigning the trigger and action each will initiate.

-	Scene Triggers - This allows you to trigger actions based on scene changes. For example:   When Camera 1 is active, start recording after 2 seconds.
-	Video - Video can monitor a video source and trigger an action when the source matches a predetermined video file. That action switches to the scene you pre-select. The trigger can also be set to engage when the source does not match or if it has changed.
-	Audio - Monitors any audio source and triggers an action when the levels go above a certain threshold (or below a threshold) for a set amount of time, it will trigger a scene switch the scene you choose. This can be used to switch camera views when specific microphones become active. 
-	Sequence - Automatically switches to a scene when another scene becomes active.
-	Idle - Switches to a preset scene if there are no keyboard or mouse inputs for a set time.
-	Time - Can trigger a scene change based on the day and time.
-	File - Triggers a scene based on the contents of a file. You can also write the name of the current scene to a file and use the contents of that same file to select the next scene.
-	Media - Automatically switches scenes based on the current state of a media source. For example, when a media source ends, switch to a title slide.
-	Region - Can automatically trigger a scene based on the cursor's position.

These are just some of the commonly used available trigger options. Next, you can set up an example trigger and action. For this example, try switching to the scene for your camera immediately after a video finishes playback.

**Example Use:**

1. In OBS, go to Tools, Advanced Scene Switcher.
2. Select the Media tab.
3. Click the + in the lower-left corner.
4. Moving from left to right, choose your media source. 
5. After "state is," choose "Played to end" from the dropdown menu.
6. Leave the next two boxes as is and then choose Camera 1 as the scene to switch to.

If you would like to try your first automated transition, go to the General tab of Advanced Scene Switcher and check to see that it is active. If not, just click the Start button.

#### How Advanced Scene Switcher is Being Used

**Gaming**
Gamers have enough to pay attention to without manually switching scenes. With Advanced Scene Switcher, gamers can automate nearly every transition in their stream while keeping their hands free.

**Video Podcasts **
Advanced Scene Switcher can keep shows moving along with automation. Producers can have countdown timers trigger intro videos which can then switch to a camera and microphone.

**Houses of Worship**
The Advanced Scene Switcher is very popular with houses of worship. Since they often rely on volunteers and can sometimes be shorthanded, this type of automation really helps.

**Sporting Events**
The fast pace of sporting events, plus the use of pre-recorded videos, graphics, and transitions, make Advanced Scene Switcher popular with sporting event streamers. It will be especially beneficial for those covering school and local sports where you don't have an entire production crew. Automating some of the switching duties can let broadcasters focus on the game.

**Pros and Cons**
Pros: It’s free. It offers powerful automation. 
Cons: The interface can be intimidating at first.

**Alternatives to Advanced Scene Switcher**
Advanced Scene Switcher appears to be the only plug-in currently available for automating scene switching in OBS.

**Key Takeaways**

1.	If you want to automate some of the switching work in OBS, Advanced Scene Switcher is a great option. 
2.	Don't be overwhelmed by the many options just choose what you will benefit from. 
3.	You may only need one or two automations to make significant improvements in your workflow. 
4.	You can always add more as you learn the plug-in and consider other places where automation can help.

 
## SOURCE DOCK PLUGIN

OBS offers a flexible interface that allows users to customize the layout. One thing that couldn't be added as a dockable panel with the ability to preview sources. The Source Dock plug-in for OBS Studio allows users to create a dockable window inside the interface for any source. In addition, each panel can be customized to provide audio level meters, volume adjustments, and media controls you can access on the fly..

**Installing Source Dock**
Source Dock can be downloaded from the OBS website. https://obsproject.com/forum/resources/source-dock.1317/. Download the version for your system (PC, Mac, and Linux ). Installation wizards are available for the Mac and Windows versions. This is the best route for most users. Otherwise, extract the .zip file and place the plug-in files in the correct folder on your computer. When you are done, restart OBS. 
 

<h2 align = "center" ><img src="/img4.png" ><h2>
<h4 align = "center"><b>Source dock includes additional controls for the sources you are monitoring. </b></h4>


**Using Source Dock**
To create a dockable panel from any source in OBS, go to Tools and select Source Dock. In the dialog box, select the source you wish to dock. Be sure the Visible box is checked. 

Check or uncheck boxes below the various features that you want to appear in the dock. These can be adjusted later.

-	Preview – This will show a thumbnail of any video source. 
-	Volume Meter – This will enable the audio level meters for the source. 
-	Audio Controls –This will allow you to adjust the levels of the sources from within the Source Dock window. 
-	Switch Scene –This will enable the source to be sent to the program output when clicked on in the panel. 
-	Show Active – This will display Active in green when the source is active.
-	Properties - This adds a button to access the properties of the source
-	Filters - This adds one-button access to filters assigned to the source.
-	Text Input – This displays a text area for notes. This could be used to display the hotkey combination used to display the sources or other information.
-	Scene Items – This displays scene layers and enables toggling of each item.

Next, click Add. The panel will appear. Click and drag it like any other panel. From there, you can adjust and rearrange the panel’s location. While Source Dock can be used with any input type, it is especially useful with live web pages and media sources.

**Using Source Dock with a Web Page**
Add a Browser Source to any scene in OBS. You can use any website you like for the URL. Once the input is created, go to Tools and select Source Dock. Add the browser source and be sure the Visible and Preview boxes are checked. Click Add and then click and drag to drop the panel to your preferred location. Now notice that if you click into the preview window in the panel, you can use your mouse to interact with the live website. You can scroll and click when the source is live or when it is inactive. This is ideal for getting up to date website information ready for display. 

**Using Source Dock with a Media Source**
Add a Media Source to any scene. Be sure that the Local File is checked. Click Browse to locate a video file on your computer. If it is a short video, you may want to check the box next to Loop. Click OK. Now once again, go to Tools, Source Dock. Choose the media source you just created. Be sure the Visible, Preview, Volume Meter, Audio Controls, and Media Controls are checked and click Add. Drag and drop the panel to your preferred location. Now you will see that you have complete control of the media source. You can start, stop, or replay the media. You can also see the audio levels and adjust them via a slider.

**Using Source Dock with a Live Video Source**
Add a Video Capture Device to any scene. Go to Tools, Source Dock and choose the Video Capture Device you just added as the source. In most cases, you will only need to check the boxes for Visible, Preview, and Switch Scenes. Click Add. Drag it to where you would like it to dock, and you now have a dedicated preview monitor that you can place nearly anywhere in the OBS interface.

#### **How is Source Dock Being Used?**

**Live Multi-Camera Productions**
It is now possible within OBS to have a preview monitor window for every camera and pre-recorded video. There would be no need for the Studio Mode Preview Window as you could see all sources simultaneously. With the Switch Scenes option selected for each input, switching would be as easy as clicking the preview of the source you wish to send to the program output.

**Houses of Worship**
Many houses of worship use multi-camera setups, and many of them are operated by volunteers. Using Source Docks, someone can configure a layout with each camera or other video source displayed in a preview panel. Then, once the service starts, the volunteer operator would only need to click the next desired input.

**Training Videos**
Some training videos rely heavily on sharing web content. With Source Dock, any Browser Source can be docked. If it is configured correctly, instructors can interact with the web page from within the Preview window. This makes displaying the web content so much simpler for instructors since the whole thing happens within the OBS interface.

**Pros and Cons**
Pros: It’s Free. It’s easy to install and to set up.
Cons: It is difficult to find any downsides to this plug-in.

**Alternatives  to Source Dock**
Source Dock appears to be the first and only of its kind. Users looking for more limited docking capabilities may want to look into the Custom Browser Docks feature in OBS.

**Key Takeaways**

1.	If you want to be able to preview input sources in dockable panels in OBS, you need to install the Source Dock plugin. 
2.	Whether you want to interact with web content via a preview window or control of pre-recorded videos, Source Dock can do it.
 

## SOURCE RECORD PLUGIN

Source Record allows you to record any source in OBS while simultaneously streaming or recording the main output of OBS. In other software and hardware platforms, this is referred to as an Isolated Output (ISO). ISO recordings are ideal for post production because they do not feature the overlays and graphics found in a full Scene and therefore can be used to easily recreate new content. Using Source Record, you can record as many sources as your computer can handle independently from the main video recording.

 
<h2 align = "center" ><img src="/img5.png" ><h2>
<h4 align = "center"><b>Source Record can be applied as an Effect Filter on available sources.</b></h4>
 

Whether you are recording the screen and a camera for video gameplay, streaming a sporting event with multiple cameras, recording a class session with various camera angles, or any other application, you may need to make a separate recording of just one source. You may want a clean copy of the screen share for example or a wide shot for post-production editing. In some cases, there are additional camera angles that won't be used in the primary production, that can be saved in the event they are needed later. The ability to record a “clean-feed” of any source can be a powerful video production tool. Source Record brings this functionality to OBS via an easy to apply filter.

**Installing Source Record**
Source Record can be downloaded for PC, Mac, and Linux from the OBS website at https://obsproject.com/forum/resources/ Download the version for your system. Depending on your system and the version you download, it may include a self-installer. Otherwise, follow the instruction to place the plug-in files in the correct folder on your computer. Once you are done, restart OBS, and you will be ready to go. Source Record will now be available as a filter for any source. 

**Setting Up Source Record**
Launch OBS normally. If you don't already have sources and scenes set up, go ahead and add one or two. Otherwise, you can work with the setup you already have. 

1. Choose the Source or Scene you wish to record by itself. There will be times that you want to record just a source by itself. However, if you're going to include more than one layer, like an overlay, you will want to set up a scene with the Source Record filter. 
2. Right-click on either a Source or the Scene you want and select Filters.
3. In this dialog box, click + to add a filter.
4. If you installed Source Record correctly, you will see it at the bottom of the list. Select it.
5. When you see Source Record in the list of filters, click on the eyeball icon next to it. This will toggle Source Connect off until you are ready.
6. In the dialog box, choose your Record Mode. This will be the trigger for your recording. For example, if you choose Streaming, Source Record will begin recording your selected source or scene at the same time.
7. Choose the path to save the files in the correct folder. 
8. Select your recording format. .mkv is recommended for most applications since, if your computer goes down, it will retain the recording up until that point. With other formats, like MP4, all the data will be lost if the recording is interrupted before it is finalized. MP4 is very popular as well for its high quality to file size ratio. 
9. Review the additional advanced settings. Note that there is an option to record a separate audio track. This could be useful if you want to record a video source, plus an external microphone.
10. When ready, toggle the eye icon back on and press close.

Now, whenever you begin to stream, record, or start whatever action you set as Record Mode, OBS will start recording your selected source or scene. You can repeat this whole process up to two more times to record a total of three isolated recordings. Another plug-in called Filter Hotkeys will allow you to start and stop Source Record with the click of a button. 

#### How is Source Record Being Used?

**Gaming**
A gamer streaming to a platform like Twitch may want to send a multi-layered output with a screen capture for the gaming system, a camera capturing their reactions as they play, and an overlay with information about the streamer. However, they may also want to be able to record their gameplay at full quality for posting on YouTube. Or, maybe the gamer wants to record full quality video from their camera for use in later post-production. With the Source Record plug-in, any source can be recorded separately at full quality.

**Houses of Worship**
Houses of worship often use volunteers to produce live video. Unfortunately, inexperienced operators are more prone to the occasional switching or camera operating error. With Source Record, it is simple to create separate recordings of up to three cameras. This way, any glitches can be edited before the service is uploaded for on-demand viewing. Social media teams could also access all the camera angles for sermon clips or music performances.

**Sporting Events**
Sports streamers have long needed a way to record an isolated output. The raw footage without any overlays is excellent for highlight reels. It is also helpful to record multiple individual cameras to capture the best view of a play. Often, the best angle is not from the camera that was streaming at the moment. With Source Record, up to three cameras can be saved independently for later review and post-production.

**Pros and Cons**
Pros: It’s free. It adds ISO capability to OBS. It’s easy to use. 
Cons: There are glitches for some users and configurations. 

**Alternatives To Source Record**
Currently, there are no other plug-ins that offer this type of functionality. This makes Source Record the only presently available option other than switching to another platform such as Wirecast, ECamm Live, or vMix.

**Key Takeaways**

1.	Source Record allows you to record as many sources as you can with your computer using OBS. 
2.	ISO recording is a popular feature in other live streaming platforms, and it adds crucial functionality to OBS. 
3.	It may be a worthwhile addition to OBS, even for those who aren't currently in need of it. The need to record a source separately could come up at any time.

 
## REPLAY SOURCE

Instant replays are a great way to enhance video content for sporting events and video gameplay. While OBS does now have built-in basic replay functionality, Replay Source offers a more powerful and flexible replay solution as an OBS plug-in.  Instant replays can add considerable production value to many types of content. Replay Source makes it easy to add this functionality to OBS and activate it with one or two keystrokes.

**Installing Replay Source**
Installing Replay Source requires a few more steps than most of the other plug-ins. However, none of the steps are particularly complicated. Moving through the steps actually goes quite quickly. The installation process requires changes to OBS settings, downloading and installing the plug-in, loading a script, and setting up hotkeys.


**OBS Settings**
Before you begin the actual installation, a few settings need to be adjusted in OBS.
1. Enable the Replay Buffer in OBS – In OBS, go to the Settings menu and select Output and then the Replay Buffer tab. If you don't see the Replay Buffer tab, check that Output Mode is set to Advanced. Next, check the box to activate Replay Buffer. 
2. Set Buffer Maximum – This is the length of the clip it will continually capture and make available for replay.
3. Set Video Format and Path – Still under the Output settings, click Recording. Here you can choose the preferred file format and the path to the directory where files should be kept. Make a note or take a screenshot of this location for a later setup step.
4. Automatically Start Replay Recording – If you will be using Replay Source regularly, you will want to set it to begin automatically so that the replay will be there when you need it. The whole concept of the feature is that, by recording continuously, you can always access the last few seconds of your recording and always be ready for a replay.
5. Load the Replay Script – In OBS, go to Tools and select Scripts. Hit + and add the Instant-Replay.lua file from the directory. Select Replay next to Media Source. Click Close.

**Installing the Plug-in**
Depending on your computer's operating system and the current version, it may include a self-installer. If you are not comfortable moving files around your computer, the self-installer would be the best option. Otherwise, follow the instruction to place the plug-in files in the correct folder on your computer. When done, restart OBS, and the plug-in should be ready to use. 

Once you have installed the plug-in and relaunched OBS, notice the Start Replay Buffer option under Controls. 

**Setting Up the Instant Replay**
1. In OBS, create a new scene and name it "Instant Replay Scene."
2. Click + under Sources and add Media Source.
3. Select Create New and name it Replay Source
4. Check to see that Local File is selected and locate the replay file. You set the directory path earlier in the OBS Settings.
5. Click OK.

**Configuring Hotkeys**
You can assign Hotkeys to all of the Instant Replay functions. You can set these up on any keys you want or even assign them to a Stream Deck or Touch Portal controller. Try using F1, F2, and F3 as an example for clarity. To set up the hotkeys, go to Settings and select Hotkeys. First, if you want to be able to toggle the replay buffer off and on with a hotkey, scroll down to Start Replay Buffer and click into the box. It will record the next keystroke or key combination and assign it to start the buffer, for now, use F1. Entering that same keystroke in the Stop Replay Buffer box will cause that F1 to act as a toggle to turn the recording on and off. 

Next, scroll down to the Replay Buffer subheading and assign F2 to Save Replay. This key will act as the trigger to save the contents of the replay buffer for playback. Finally, scroll down to Instant Replay and assign it to F3. Click Apply and OK.

**Using Instant Replay**
There is a lot of flexibility when it comes to how to use instant replays in your production. Since Instant Replay is configured as a source, you can add it to the scene, and crop, resize and move the window within the scene. Once you have it set up, you can save and playback a replay at any time. With the example setup, you would just need to click F1 to start the Replay Buffer. Then, when you are ready to share a replay, click F2. OBS will save the video clip in the buffer, the length based on the settings entered earlier. Finally, F3 will begin the replay.

#### How is Replay Buffer Being Used?
**Gamers**  
Gamers are quickly learning how to massively upgrade their production values on Twitch and YouTube using Instant Replay. There is a lot to think about when running a stream and focusing on the game. Instant Replay's use of hotkeys means that the gamer can get a replay live on the stream with just a couple of clicks of the keyboard or Stream Deck. Gamers are also using the Replay Source alongside other plug-ins to add filters and effects automatically when launching a replay.

**Sporting Events**
While the Instant Replay plug-in does not offer some of the more advanced features found in software like vMix or Wirecast, it can add some excitement to a sports broadcast or stream. While this solution does not let you select from multiple camera views like the more advanced software, producers can get impressive results using filters and other plug-ins. 

**Pros and Cons**
Pros: It’s free and easy to use. It includes multiple setup options. It has been well integrated with OBS.
Cons: Setup is not as simple as other plug-ins, and it can take some time and effort to get everything working properly, Can only replay OBS main output and not specific sources.

**Alternatives To Replay Source**
OBS – As mentioned, OBS does have replay functionality built-in. Instant Replay builds on that framework to create a more straightforward and more powerful tool.

There do not appear to be any other OBS-based alternatives to Replay Source other than OBS's built-in option. However, there are some options that work outside of OBS to capture the stream locally and have it ready for replay.

**Key Takeaways**

1.	If you want instant replay in OBS, Replay Buffer is the best option.
2.	Its operation is seamless and straightforward once you get everything set up. 
3.	Just be aware that getting everything configured may take some time.



## AUDIO MONITOR PLUGIN
OBS is a great tool, but it has some limitations, especially when it comes to audio monitoring and control. An audio feature desired by many streamers has been a way to create a separate headphone mix that will allow users to monitor and send any source within OBS to any audio device they choose.

Over the years, there have been several workarounds, but the Audio Monitor plugin for OBS offers all the functionality producers need in an easy-to-use interface. Audio Monitor gives you the ability to send the audio of any OBS source to any audio device just by adding the Audio Monitor filter to the source. With this, you can create your own custom headphone or monitor mix or even create a separate mix to feed your host or guests headphones. The Audio Monitor plugin will be shown with several examples in this book including how to use OBS with Zoom and also creating closed captions with Web Captioner.

 
<h2 align = "center" ><img src="/img6.png" ><h2>
<h4 align = "center"><b>Audio Monitor can be shown as a dock inside the OBS interface.</b></h4>


**Installing Audio Monitor**
Audio Monitor can be downloaded for PC and Mac, from the OBS website https://obsproject.com/forum/resources/audio-monitor.1186/. Download the version for your system. Depending on your system and the version you download, it may include a self-installer. Otherwise, follow the instruction to place the plugin files in the correct folder on your computer. Once you are done, restart OBS, and you will be ready to go.

**Using Audio Monitor**

1. Select any source with audio in the Audio Mixer.
2. Click on the settings icon at the bottom of the source in Audio Mixer.
3. Select Filters.
4. Under Audio Filters or Audio/Video Filters, Press the + and add Audio Monitor.
5. Select the device to which you wish to send the audio from that source. You can send it to any device connected to your system. That includes audio interfaces and even virtual devices like a Virtual Audio Cable.
6. You can adjust the volume levels. This level will only impact the level of the source to the selected device.
7. You can add as many Audio Monitor filters as you wish and send any source to as many devices as you want.

**Adding the Audio Mixer Dock**
Go to the View menu and click Docks and select Audio Monitor. The Audio Monitor panel can be docked within the OBS interface just like any other panel. You can also move it to the same panel as the default mixer and use a tab to switch between them.  While the two audio mixers look similar, the Audio Monitor panel has an extra gear icon and meter on the left. By pressing the gear icon, you can choose to display all available audio sources or just those available in the current scene.

Within the Audio Monitor panel, the sliders can adjust the output levels from that source to your selected audio device. That is unless you locked the level when you set up the filter. There are additional options within the settings menu. One handy feature is found by clicking on the gear icon and selecting Outputs. As OBS allows you to record up to six audio tracks, this feature will enable you to preview and control the output levels for each track.

#### How is Audio Monitor Being Used?

**Gaming**
Audio Monitor is a great tool for gamers streaming to Twitch, YouTube, or other platforms since it allows them to send one mix to the stream and another to their monitors or headphones. Most gamers would like to control exactly what is going into their headphones and make it different from what viewers will hear. For example, gamers may or may not want to listen to their own vocals. They might want a different level for game audio. Some might even want to add music to the stream but leave it out of their mix.

**Video Podcasts and Programs**
Any production with a guest or multiple hosts can benefit from Audio Monitor. If the host is also operating OBS, they may need to be able to monitor some audio that the guest does not need to hear in their headphones. Audio Monitor allows users to set up a separate mix assigned only to the audio device feeding the guest's headphones. The host can also set up their own custom mix that may differ from what listeners will hear.

**Live Entertainment**
Live streamed music and entertainment are more popular than ever. Audio Monitor gives OBS the functionality to handle the unique challenges of live events, especially music. With Audio Monitor and the proper audio devices, you could provide separate monitor mixes for musicians, vocalists, hosts, and producers, all within OBS.

**Pros and Cons**
Pros: It’s free. It’s easy to install and has a great dockable interface. It’s easy to use it with virtual audio cables with software like Skype or Zoom. 
Cons: The layout and function of the interface can take some time to understand. As a relatively new plugin, there are still some bugs.

**Alternatives To Audio Monitor**
VoiceMeeter Virtual Audio Mixer – Prior to the release of the Audio Monitor plugin VoiceMeeter was the standard for many users. Unfortunately, it was more challenging to set up and operate. Also, as opposed to being a plugin running within OBS, VoiceMeeter is a stand-alone application.

**Key Takeaways**

1.	If you want greater control of your audio monitoring in OBS, Audio Monitor is a great plugin. 
2.	It can take a little time to learn but is far less complicated than VoiceMeeter. 
3.	Audio Monitor is ideal for complex workflows such as connecting OBS with Zoom.

 

## FILTER HOTKEYS

OBS Studio comes standard with filters. You can add filters to any source, scene, or audio source. However, there was no way to quickly and easily turn these filters on and off. Filter Hotkeys adds the ability to turn filters on and off using assignable hotkeys or even a Stream Deck or Touch Portal controller. Filter Hotkeys make it easier to control your favorite filters. 

**Installing Filter Hotkeys**
The required files are available from the OBS website at https://obsproject.com/forum/resources/obs-filter-hotkeys.1125/. Filter Hotkeys is actually a script rather than a plug-in, so the installation process is a little different. 
1. Click download, and it will send you to the GitHub page. 
2. Scroll down to assets and download the zip file.
3. Extract and copy the .lua files to the directory where your OBS scripts live.
4. In OBS, go to Tools, Scripts.
5. Press +. It will automatically open to the correct folder where you pasted the scripts. Select both script files and click to open
6. Before you close this dialogue window take note of the note in the description where it reads, "Note: 0 - means disable filter, 2- enable, 2 - toggle, 3 - hold." You will need to know these later when setting up your hotkeys.

**Using Filter Hotkeys**
1. Create a source or choose an existing source, right-click on it and select Filters.
2. Use the + at the bottom of Audio/Video Filters or Effect Filters and add one or more filters. Take note of the names you give the filters. You will need those later.
3. Go to Settings, Hotkeys.
4. Find your filter by scrolling or by searching for it in the search box at the top. 
When you find it, you will see that there are four fields where you can set hotkeys. They are labeled 0, 1, 2, and 3 and correspond to the note you saw in the script dialog box. The hotkey you set for 0 will disable the filter. The hotkey for 1 will enable it, 2 will toggle it on and off, and 3 will hold the filter on as long as you hold it, at which point it will turn off.

#### How Filter Hotkeys is Being Used
OBS users have discovered some creative uses for Filter Hotkeys. Here are some examples.

A streamer wanted to be able to add EQ and Reverb to his microphone to deliver a spooky evil laugh. With Filter Hotkeys, he can toggle it on and off with one keystroke.

A gaming streamer needed the ability to toggle the Chroma Key to alternate from her green screen to a replacement background. She was able to set up the filter and activate it with a hotkey

Another streamer uses Filter Hotkeys to enable a Scroll filter. A text source list of his supporters and other credits is set up, and when ready, the host can hit one key to start the scroll and another to end it.

Producers with multiple hosts and guests use Filter Hotkey to turn audio filters on and off. Without it, it can be difficult to make audio adjustments on the fly. However, with Filter Hotkeys, one keystroke can turn on gain adjustment, a noise gate, noise suppression, or compression. This can at least temporarily fix audio issues at least until further adjustments can be made.

**Pros and Cons**

Pros: Free. Easy to use once set up.
Cons: With no auto-installer package, setup and configuration can be difficult.

**Alternatives to Filter Hotkeys**
Filter Hotkeys appears to be the only plug-in currently available for toggling filters with hotkeys in OBS.

**Key Takeaways**

1.	Not everyone needs the power to toggle filters with hotkeys. However, if you do, Filter Hotkeys is the only option for OBS. 
2.	Fortunately, it is extremely easy to set up and use.




## ANIMATED LOWER THIRDS

Have you ever wanted to control your lower thirds on the fly? With Animated Lower Thirds you can control four different lower thirds simultaneously with an easy to use dockable control panel. Even better, you can include logos, have total control over formatting, and trigger the lower thirds using hotkeys.

**Installing Animated Lower Thirds with Dockable Control Panel**
You can download the necessary files for Animated Lower Thirds with Dockable Control Panel from the OBS website. https://obsproject.com/forum/resources/animated-lower-thirds-with-dockable-control-panel.1057. It is available for Windows, Mac and Linux. This is another add-on that is not actually a plug-in, so the installation instructions are somewhat different. 

1.	Download and extract the .zip file. Next, you will need to move that "Lower-Thirds" folder into the OBS program files folder. You can find that location by opening OBS. Once OBS is running, right-click the icon and the taskbar, then right-click on OBS and click properties. Next to Target, you can see where your program files are. 
2.	Next, go into the "Lower-Thirds" folder and then the "lower thirds" folder.
3.	Get the local URL of control-panel.html by clicking it to open in your browser. Copy the URL from the browser's address bar. 
4.	In OBS, click View, Docks, Custom Browser Docks.
5.	Under Dock Name, give the dock a name, in this case, Lower 3rd.
6.	Next, paste the URL you just copied into the URL field. Hit Apply and Close.
7.	You will see the dock on the screen. You can drag and drop it anywhere in your interface

**Setting Up Hotkeys for Animated Lower Thirds with Dockable Control Panel**

1.	In OBS, go to Tools, Scripts.
2.	Click the + sign in the lower-left corner. That will take you to the default .lua script location. However, you will need to navigate to the folder where you moved the downloaded Lower-Thirds folder. Click into the "lower thirds" folder and select the lower-thirds_+hotkeys.lua file. Click Close.
3.	Go to Settings, Hotkeys
4.	Scroll down until you see Lower Third Switch #1, #2, #3, and #4. Type your selected key or keys into the fields. These will now toggle your lower thirds on and off.

 
<h2 align = "center" ><img src="/img7.png" ><h2>
<h4 align = "center"><b>Lower thirds can be edited in the management panel.</b></h4>


**Completing Setup for Animated Lower Thirds with Dockable Control Panel**
1.	Set up a source for your lower thirds in OBS studio. Click + under Sources, select Brower and name it Lower 3rd.
2.	Ensure that the box next to Local file is checked.
3.	Click the Browse button and go to the "Lower-Thirds" folder you downloaded and moved earlier. Next, click into the "lower thirds" folder, click "browser-source," and click open.
4.	Double-check the width to ensure it matches your current canvas resolution,
5.	Highlight the text in the Custom CSS section and delete it.
6.	Be sure there are checks in the boxes next to Shutdown source when not visible and Refresh Browser when the scene becomes active.
7.	Click OK.

**Configuring Animated Lower Thirds with Dockable Control Panel**
1.	Turn on the Main settings toggle at the top of the Lower Thirds control panel.
2.	There are also toggle sliders next to each of the four lower thirds. We will later assign hotkeys to turn these on and off as needed.
3.	Click the + next to Main Settings to access the global settings for all the lower thirds.
4.	The Global Times field sets the transition time, visibility time, and the amount of time until the lower third starts over.
5.	Select the theme from the three options.

**Using Custom Fonts**

If you would like to use custom fonts in your web browser, go to fonts.google.com and choose a font. Click Select this style next to the font and style you wish to use. In the column at the right of the screen, check the radio button next to @import. Highlight and copy the text under "CSS rules to specify families." 

Back in OBS, in the Animated Lower Thirds panel, click the + next to  Main Settings to expand the window. Next, click on the Customs tab. Paste the text you copied into the field next to Custom Font. Next, go back to your web browser and copy in the other box. In OBS, paste that in the other field next to Custom Font. Hit the +, and the font is installed. You can repeat the process to add additional fonts.

**Adding Logos**

In order to add logos, you need first to place those graphics in the correct folder and give them the correct name inside the Lower-Thirds folder that you moved into the OBS program files folder, open logos. To add logos, you must replace the existing files with files of the exact same names. For example, one of your logos will need to be named logo_1.png and replace the current logo_1.png file in the folder. In addition, they must be ping 24 with transparency.

**Setting Parameters for Individual Lower Thirds**

1.	Toggle the selected Lower Third on using the slider at the top.
2.	Click the + to expand the settings options
3.	Here, you can toggle the logo on and off, set the background color and text colors, add a drop shadow, alignment, size, position of the lower third, and more.

#### How Lower Thirds with Dockable Control Panel is Being Used

**News Broadcasts**

Those producing streaming or broadcast news programming with OBS love the convenience of triggering and modifying lower thirds on the fly. Since the settings are in a dockable panel, it is fast and easy to make changes or add new text or logos right from the OBS interface. With hotkeys configured, any of these lower thirds can be triggered from the keyboard.

**Online Meetings**

Users add a professional touch to their appearance in online meetings using animated lower thirds. With OBS connected to Zoom, Microsoft Teams, or other video conferencing platforms, hosts can use text and logos to introduce themselves or guests and include additional on-screen information with just a couple of keystrokes.

**Houses of Worship**

Live stream producers can add professionalism to their services with lower thirds. These can be used to introduce worship leaders and other people involved in the services.

**Pros and Cons**

Pros: Free. Extremely customizable.
Cons: Multi-step installation can be overwhelming.

**Alternatives to Animated Lower Thirds with Dockable Control Panel**

There are not currently any plug-ins or other options that match the power and features of Animated Lower Thirds with Dockable Control Panel. However, simple lower thirds can be created in OBS just by creating additional layers for graphics and text and including them as part of a scene.

**Key Takeaways**

1.	A lower third is a common graphic used to display information about a video in the lower third of the screen. 
2.	Great-looking lower thirds are easy to manage, edit, and trigger, with the Animated Lower Thirds plugin. 
3.	This plugin includes an easy to use Dockable Control Panel.

 


## BACKGROUND REMOVAL


Background removal tools, which allow you to remove or replace a video background without a green screen, are more popular than ever. They are showing up as an included feature in popular video conferencing applications like Google Meet and Zoom. However, background removal was not available in OBS directly until this plug-in was developed. Fortunately, with the Background Removal plug-in for OBS studio, you can remove backgrounds without a green screen. It is easy to set up and absolutely free.

**Installing Background Removal** 
Background Removal is available for download for Windows, Mac, and Linux from the OBS website at https://obsproject.com/forum/resources/background-removal-portrait-segmentation.1260. Clicking the download link will take you to the GitHub page. 

Unfortunately, there is no installer package available, so you will need to unzip the files and place them in the correct folders with your OBS program files. Instructions are included on the page. The actual downloads are located under “assets” at the bottom of the page.

**Using Background Removal**
Background removal is available as a filter. You can add the filter to any video source.
1. Create a video source or choose one that is already available in OBS.
2. Right-click the source and select Filters.
3. Under Audio/Video Filters, click +.
4. Select Background Removal from the list.

 <h2 align = "center" ><img src="/img8.png" ><h2>


**Background Removal Settings**
If everything is correctly installed, you should see your video source in the dialog box window. Below that, you will see the adjustable settings for the filter. You can perfect the effect with the following sliders.

-	Threshold - Adjusts the required color differentiation between the subject and background. If you turn this all the way down, you will likely find that the subject itself is removed from the image. However, if it is too high, you will see a sort of halo around the subject, and eventually, the entire background will show.    
-	Contour Filter – Adjust the tightness of the contour around the subject that separates it from the background.
-	Smooth silhouette – The higher the setting, the more it will try to smooth the edges of where the subject meets the removed background. If you turn it all the way down, the edges will be rough and pixelated. You can see them smooth out as you move the slider to the right.
-	Feather blend silhouette – The higher the setting on this slider, the more the filter will try to soften the edges of the subject.
-	Background Color – Selects the color that will be shown in place of the original background image. This can be any color, but if you plan to use a chroma key to replace the background, you should set this to the appropriate shade of green.
-	Segmentation Model – Selects the method of differentiating the background from the subject. You may want to click through the options to see which one works best for your use.

As with any background removal tool, you will likely need to experiment for the best results. If you are having trouble getting the results you want with just the filter settings, take a look at your physical environment. For example, you may need to add more light on your subject or increase the distance from the background to make it easier for the filter to make the differentiation.

Once your background has been removed and replaced with a single color you can use the chromakey filter to make the background transparent. 

 
<h2 align = "center" ><img src="/img9.png" ><h2>
<h4 align = "center"><b>The Threshold slider is one of the most important adjustments to fine tune your removal of the background.</b></h4>

##### How Background Removal is Being Used

**Online Meetings/Video Conferencing**
While background removal is becoming standard in many video conferencing platforms, many users prefer to connect OBS to the video platform for better control. This enables users to have finer control of background removal from within OBS.

**Gamers**
Many gamers like to remove their background from the webcam, but green screens are not always a viable alternative. With a bit of experimentation, they can get green screen quality results without the green screen.

**News** 
Newscasts have been using green screens for years, especially for weather and sports. Now producers without access to green screens can remove the background from behind the talent, replace it with green and get the same effect.

**Pros and Cons**
Pros: It’s free. It does not require a green screen. 
Cons: Like all background removal filters, the quality will largely depend on things like lighting and background. If you can get everything just right, you may not get the results you are looking for.


**Alternatives to Background Removal**
With a green screen, users can use the built-in chroma key filter for the same purpose.

**Key Takeaways**

1.	It will take some experimentation to get results nearing those of a properly used green screen. 
2.	Ithe right setting, this is a powerful background removal tool that works great inside OBS.




## CLOSED CAPTIONS FOR OBS

Adding captions to your production is a great way to improve the accessibility and reach of your video content. Closed captions can remove language barriers, make content accessible for those with hearing limitations, and allow people to watch videos when it isn't practical to have the sound on. Captioning also offers SEO (search engine optimization) benefits as Google and other search engines can index the captions and improve your performance in search results.

Given the many advantages of captioning, adding this feature to nearly any video production makes sense. However, while some video platforms offer captioning, many streamers like to control both the content and layout of captions. This is especially true for broadcasts with many on-screen components (titles, graphics, etc.) that could be blocked by auto-generated captions. There are multiple closed captioning solutions available for OBS, but Web Captioner is one of the easiest to use because it allows OBS users to add closed captions to in just a few steps. There are two options for using the platform. The simplest option is to use Web Captioner in the Google Chrome browser and capture the window in OBS. The more advanced method will encode the caption data into the live stream. 

 
<h2 align = "center" ><img src="/img10.png" ><h2>
<h4 align = "center"><b>Web captioner shown overlaid on top of the OBS interface.</b></h4>

**Getting Started with Web Captioner - Option 1 - Screen Capture**

Web Captioner is technically not a plug-in for OBS. However, it is covered here since it is free and it adds a superior level of functionality to most plugins that are currently available. Since Web Captioner is not a plug-in, there is no installation required. Instead, just go to webcaptioner.com from your Chrome Browser. Please note that Web Captioner currently only works in Google Chrome. That is because it uses the Web Speech API, which is only supported by Chrome. 

Just click the "START CAPTIONING" button to begin. This click will take you to a mostly black screen. Next, press the "Start Captioning" button at the bottom of this page. The first time you use this web-app you will be asked to give permission to access your microphone. Now any system audio from your microphone, audio interface, or a pre-recorded file will be captured, and Web Captioner will create text from any dialog. If you would like to route audio out of OBS and into Web-Captioner you can do so using a virtual audio cable and the Audio Monitor filter you learned about earlier in this book.

Getting this into OBS is as simple as adding a new Window Capture source and choosing the Chrome window showing Web Captioner. That will bring in the entire window, and it can be used like any other source. However, it isn't very likely that most users will want to show a full screen of captions. So instead, you can use OBS's built-in tools to crop, resize, and move the window.

If you want access to more tools to customize your caption text, return to your Chrome browsers and Web Captioner. Click on the three-dot menu at the bottom right of the screen to launch the menu and click Settings. Here you can adjust nearly every aspect of the look and format of the caption text. Under "Appearance," you can change fonts, text color, line height, letter spacing, alignment, capitalization, and even background color.

On the General tab of the settings, you can control what will happen when there is no audio. For example, when you or your video host stop speaking, you can have it do nothing and hold on to the last words, add between one and five line breaks, or clear the entire transcript.  If you want to save your settings, just sign up for a free account and be sure you are signed in.

**Using Chroma Key for a Transparent Background**
If you would like your captions to display with a transparent background in your OBS production, you will need to take steps in the Web Captioner Setting and in OBS.
1. In Web Captioner, open the Settings menu and select the Appearance tab. Be sure the text color is correct for your needs. 
2. Scroll down to Background Color. Change it green or whatever key color type you wish to use for your chroma key. If you aren't sure, type "0 177 64" into the RGB fields.
3. In OBS, right-click on the Window Capture source you set up for Web Captioner. and select Filters.
4. In Effect Filters, click + and select Chroma Ke,y and give it a name. Click OK.
5. Click on your new filter in the Effect Filters box. If you used green, you should see it already replaced with grey. Below you can change the Key Color Type and fine-tune the chroma key.

**Getting Started with Web Captioner - Option 2 - Embedded Closed Captioning**
While Web Capture is not a plug-in, this method of use does require the installation of the OBS Websocket plug-in. The Websocket plug-in is covered elsewhere in this section. This method will encode closed-caption data into your stream. While you won't see the text in OBS, viewers will be able to use the "CC" button to turn on captions on platforms like Facebook, YouTube, and Twitch. 

Note: This method requires OBS Studio Version 26.1 or later.

1. Be sure the WebSocket plug-in is installed and restart OBS.
2. In OBS, go to Tools and select WebSockets Server Settings.
3. Enable the WebSockets server and then set the port number. Adding a password is optional but recommended.
4. Return to Web Captioner in your Chrome web browser and open the Settings menu.
5. Select the Channels tab and select OBS Studio. Enter the port number and password you previously added in OBS.

#### How is Web Captioner Being Used?
**Educational and Instructional Content** 
Many instructors teaching in online virtual classrooms know that captions can be critical for many different types of learners. Teachers often want to control their captions and feel uncomfortable with anything auto generated outside their control. They also might be using a teaching or video conferencing platform that does not provide auto-captions. More instructors are starting to use OBS and connecting it to Google Meet, Zoom, Skype, Microsoft Teams, and other video conferencing software.

**Conferences and Events**
Even after the pandemic, virtual and hybrid conferences and events will continue to allow people to connect to resources and colleagues without the cost and time associated with travel. The online virtual component becomes far more accessible when live captioning is available. This benefit may be significant for attendees traveling from other countries who don't speak the primary language of the conference. People who are less than fluent can have an easier time if they can see the text simultaneously.

**Houses of Worship**
Houses of worship strive to be accessible to as many people as possible. With more people than ever attending online, they need platforms like Web Captioner to ensure accurate captions for sermons and other spoken-word content.


**Pros and Cons**
Pros: It’s free. It has Multiple setup options. It’s easy to use with OBS. 
Cons: No punctuation unless explicitly spoken (i.e., question mark.), Some users find it frustrating that the Web Captioner Chrome window needs to remain open for the screen capture method to work.

**Alternatives To Web Captioner**
Closed Captioning via Google Speech Recognition (https://obsproject.com/forum/resources/closed-captioning-via-google-speech-recognition.833/)
This plug-in provides closed captioning via the same Google Cloud Speech Recognition API as Web Captioner but in a standalone OBS plug-in. Unfortunately, since it uses Twitch's built-in caption support, it only works on that platform.
Caption.Ninja

This bare-bones option works similarly to Web Captioner but only allows for the Screen Capture method. It also lacks any customization settings, so you get black letters on a white background as your only option.


**Key Takeaways**
1.	Web Captioner is an easy and powerful way to add live captioning to your video production. 
2.	Web Captioned can be used to add captions on-screen with screen capture or embedding captions into your production via a web-browser in




## WORKING WITH VIRTUAL AUDIO CABLES


OBS has become a popular production solution for people who use video communications software such as Microsoft Teams and Zoom. Many people who use video communications or web-based live streaming software, would like to increase the quality of their production, but only have the ability to use a webcam and microphone as audio visual inputs. This is where virtual video and audio cables come into play with OBS. OBS is capable of outputting a virtual video camera which can be used with software like Zoom as the webcam input. OBS is also capable of using virtual audio cables to connect audio from OBS to other applications on the same computer. These virtual audio and video connections allow you to use OBS with any software that leverages a standard webcam and microphone input.

Use cases for virtual audio and video connections vary widely. One of the most popular ways to use a virtual webcam output from OBS is with software such as Zoom. Zoom does offer some visual enhancements such as blur effects, but OBS offers much more flexibility. The latest version of OBS now includes a usable USB webcam driver by default which you can select inside of any software that uses webcams. Using the Start Virtual Camera button inside of OBS, you can send the video directly from your OBS output to any software that is using the OBS Camera webcam input.

 
<h2 align = "center" ><img src="/img11.png" ><h2>
<h4 align = "center"><b>Connecting OBS and Zoom is easiest if you have two monitors.</b></h4>


You can also bring video from Zoom back into OBS for live streaming and recording. To bring video from Zoom back into OBS you can use a desktop or window capture source. Many users prefer recording Zoom meetings and interviews with OBS because they can control the bitrate and therefore the quality of their video recordings. After much testing, the StreamGeeks have determined that most recordings made with Zoom are less than 2 Mbps. For reference a good quality YouTube video would be at least 4-6 Mbps. Using OBS will allow you to record video in a higher quality and record locally on your harddrive without Zoom’s compression settings. You can also record individual sources for use in post production after an event. This is ideal if you have a nice camera that you do not want to have compressed by Zoom’s cloud-based recording process. 



<h2 align = "center" ><img src="/img12.png" ><h2>
<h4 align = "center"><b>Connecting OBS and Zoom only has to be done once and it is easy to use once it is configured.</b></h4>

Setting up virtual audio cables to work with Zoom and OBS is more complicated than using the built-in virtual camera feature. OBS does not offer built-in virtual audio cable support at this time and therefore, you will need to download virtual audio cables to send audio from OBS to other applications on your computer. By using virtual audio cables, it is possible to record both audio and video from applications such as Zoom and Microsoft Teams. Using virtual audio cables allows you to enhance the audio coming in and out of OBS with audio plugins and tools that are not available in many video communications tools.

You can download two virtual audio cables for free from VB-Audio.com for your Mac or Windows computer. The VB-CABLE drivers are donationware, so they will ask you to make an optional donation to the developers. The default installation package includes two virtual audio cables, because you will require one for sending audio and one for receiving audio. Once they have been installed on your computer, you should restart. The next time you open Zoom or a similar application you will see new virtual audio cables for input and output inside Zoom when you open the microphone and speaker area. 

Inside of Zoom, you can select CABLE Input for your microphone and CABLE Output for your speaker. This will allow you to send your microphone audio into Zoom using the virtual CABLE Input and receive audio into Zoom using the CABLE Output. In order to send audio out of OBS you will need a plugin called Audio Monitor. The Audio Monitor plugin adds an important Audio/Video Filter to OBS which allows you to output audio from any number of sources. Find the audio sources you would like to send into Zoom and apply the Audio Monitor Filter. Inside the filter select the CABLE Input option. You have the option to mix audio by reducing the volume of each input that is being sent into the virtual cable. 

Next, inside of OBS, you will want to create a microphone input to bring the audio from Zoom into OBS. You can do this by opening an Audio Input Capture source and selecting Cable Output. An easy way to test if everything is working, can be done within Zoom’s settings area under Audio. You can click the Test Speaker button to send audio into OBS and make sure you are seeing levels for the audio. When you do this you should be hearing the test audio in your speakers or headphones. If not, check the Audio section of the OBS settings and check which device you have selected as your Monitoring Device. Your Monitoring Device is the device OBS will send the audio to. Next you should check to see if your audio sources from OBS are making it into Zoom. This can be done by playing audio in OBS and checking to see if you are receiving the audio levels inside of Zoom. Zoom has a handy audio monitoring feature inside the microphone to let you know when it’s receiving audio from the selected microphone source. 

Connecting OBS and Zoom can significantly increase your video and audio quality for meetings and interviews. If you have a studio or multiple cameras, you can now seamlessly switch between them in Zoom meetings. You can also use animated lower thirds to make your presentations look more professional. Another popular reason to use OBS with Zoom is the ability to play videos directly into Zoom without having to jump into a Screen Share session. In the Udemy course files, there is a transparent meeting countdown timer you can use in an upcoming meeting with this setup. The opportunity to have more fun and look more professional in online meetings is greatly enhanced by the use of OBS. 

**Key Takeaways:**

1.	OBS can be used to send audio and video directly into software such as Skype and Zoom. 
2.	OBS has a default Virtual Camera feature which allows you to send video to other applications using a virtual webcam.
3.	OBS does not have a default virtual audio cable solution and therefore a virtual audio cable driver is necessary to send both audio and video from OBS to other applications like Zoom.

