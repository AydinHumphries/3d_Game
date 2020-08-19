# 3d_Game

This is a 3d game I have created on Godot (Gd) following the tutorial series by BornCG: https://www.youtube.com/watch?v=VeCrE-ge8xM. It is for me, part of a learning curve to begin my own project. My end project involves a virtual nightclub where users create avatars to move around and interact with DJ equipment or arcade style machines that trigger sound effects. Although I created a 3d game on Godot thanks to BornCG, I do not believe it will be sufficient to use Godot alone for the extended project. That is because of complications with audio parameters I wish to introduce.

"Godot Engine is a feature-packed, cross-platform game engine to create 2D and 3D games from a unified interface. It provides a comprehensive set of common tools, so that users can focus on making games without having to reinvent the wheel. Games can be exported in one click to a number of platforms, including the major desktop platforms (Linux, macOS, Windows), mobile platforms (Android, iOS), as well as Web-based platforms (HTML5) and consoles."
https://github.com/godotengine/godot

You can Gd install here: https://godotengine.org/download/windows

I understand Gd has built in audio features which I admittedly don't know much about ( https://docs.godotengine.org/en/stable/tutorials/audio/audio_buses.html ). I am just concerned that these may not be the best possible solution as Pure Data for instance was a software designed specifically for audio manipulation: 

"Pure Data is a visual programming language developed by Miller Puckette in the 1990s for creating interactive computer music and multimedia works. While Puckette is the main author of the program, Pd is an open-source project with a large developer base working on new extensions."
https://en.wikipedia.org/wiki/Pure_Data

You can click on the Macintosh or automatic installer link for windows here: http://msp.ucsd.edu/software.html

I have been using Pd 2+ years, I'm just more confident with the language when it comes to manipulating audio parameters. Gd I picked up at the end of last month. My projects on Pd, though, involve two aspects I don't think you could do as well on Gd: 

1. audio synthesis to create new sounds, mostly I base my models around this guy's work on that.
https://www.youtube.com/watch?v=I88Cxi86Zu8&list=PLqJgTfn3kSMW3AAAl2liJRKd-7DhZwLlq

2. complex sequencing system that allows you to arrange musical material for example into specific samples or harmonies/rhythms/general patterns. It is hard to elaborate more on these things unless you understand music theory but here's an example of something I did in the past:
https://youtu.be/XGegDF9OzU4

A new project will involve a second city style of game where users can move an avatar around a virtual setting and interact with on-screen visual objects that will send the signal to pd to organise musical responses in the style I created earlier projects.

Anyway, at the moment I am not trying to replicate 1 and 2 in the above. I am trying to create a simple coin chink sound on the 3d Game I already created. I'm aware that this is relatively easy to do on Gd alone. However, I want to use Gd script to control Pd to do it. This is merely a starting point for controlling more complex audio parameters on Gd via Pd. Most of the files are native to Gd, however there is one Pd file in there that contains the patch for controlling the coin chink wav file. That's the one I want to use for now to control the coin chink through Gd. It is located in the "Audio" folder. The Godot project file is in the main folder.

Some relevant links:
- https://docs.godotengine.org/en/stable/classes/class_os.html
- http://write.flossmanuals.net/pure-data/send-and-receive/
- https://puredata.info/docs/faq/virtualmidi
- https://docs.godotengine.org/en/3.2/classes/class_packetpeerudp.html
