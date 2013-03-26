---
layout: post
category: "work"
tags: [note, Xorg]
---
{% include JB/setup %}
In this article, we focus on some basic and foundational introduction about the X11 related topics in our linux experience.  
####Xorg Server ####
There are mainly two sub\-sections in the Xorg Server section. firstly, I will conduct some introduction and explanation about the history and roles Xorg take in our hole GUI system. secondly, I'll give a practical example to show the process of problem trackback and solved. 

#### Login Manager or Display Manager ####
To some kinds, when you setup the xorg server and install the Window manager or Desktop Environment you could start the X11 system with just a command `start x`. But if you want the show the GUI graphic system all the way, and you won't want to start the x system in console, you need the help of **Login manger*, the default login manager for the Gnome is gdm. and correspondly, for Fluxbox, the slim is an ideal choice. Just with these simple line, you could use it.  
	
	equo install x11-misc/slim
	vim /etc/conf.d/xdm
and the make the change of the following:

	---
	DISPLAYMANAGER="slim"
	---
finally, you should add the xdm to default run\-levels.
	rc-update add xdm default
