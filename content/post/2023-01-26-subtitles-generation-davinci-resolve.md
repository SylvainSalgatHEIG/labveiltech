---
layout:     post
title:      "Subtitles generation with Davinci Resolve"
subtitle:   ""
description: "Subtitles generation with Davinci Resolve"
date:       2023-01-26 11:00:00
author:     "Sylvain Salgat"
image:      "/img/2018-02-09-vim-tips/matrix.jpg"
published: true
tags:
    - HowTo
    - DavinciResolve
URL: "/2023/01/26/subtitles-generation-davinci-resolve/"
categories: [ Tips ]
---

## What am I trying to learn through this experience?
As a film editor, one of the most tedious and time-consuming tasks can be transcribing audio to text in order to create subtitles for your videos. While many video editing software programs, such as Adobe Premiere, have built-in transcription tools, the same feature is not always available in other programs, such as DaVinci Resolve. In order to streamline the editing process, many editors are turning to AI-powered transcription software as a solution. One such software is StoryToolkitAI, a plugin that can help editors work more efficiently by automatically transcribing audio and allowing them to search transcripts semantically with the help of AI. This plugin can be integrated with DaVinci Resolve, which makes the process of creating subtitles a lot more manageable.

## Which tool am I going to use for this experience?
I found StoryToolkitAI, an open-source plugin offers a variety of features that can aid in the film editing process. The ability to automatically transcribe audio in multiple languages and translate it to English on a local machine can save a lot of time and effort compared to manual transcription. Additionally, the ability to search transcripts semantically using AI can make it easier to find specific segments of dialogue within the transcript.

## How did my experience go?
The integration with DaVinci Resolve Studio 18 via API allows for easy navigation and marking of timelines using the transcript. The feature of transcript segment groups allows grouping of transcription segments similar to marking in NLEs, and the ability to import subtitles directly into Resolve makes the workflow more efficient.

The ability to convert existing SRT files to transcripts and use them in the tool, export transcripts to multiple formats, and batch transcriptions using transcription queuing are additional useful features. The plugin also includes the ability to perform partial re-transcription of timelines/videos/audio files, which can come in handy in case of errors or mistakes.

Overall, the StoryToolkitAI plugin is a powerful and efficient tool for film editors, and could be a great asset in streamlining the editing process and save a lot of time and effort.


## vim graphical cheat sheet

![](//img/2018-02-09-vim-tips/vi-vim-cheat-sheet.svg)
<!--more-->
## Vim Jumps

* ^ — Move to start of line
* $ — Move to end of line
* b — Move back a word
* w — Move forward a word
* e — Move to the end of the next word
* Ctrl-o and Ctrl-i to go to the previous/next location you jumped to
* ``(two backticks) jump back to where you were
* gi go back to the last place you inserted a text and enter insert mode

## Vim Navigations

* { and } jump paragraph back and forth
* Ctrl-F/B move one screen back and forth
* Search the word under cursor, then n/p to jump to next/previous 


## Enable Vim mode in bash
vi ~/.inputrc
set editing-mode vi

## Enable system clipboard upport

See if system clipboard is supported:     
```
$ vim --version | grep clipboard
-clipboard       +iconv           +path_extra      -toolbar
+eval            +mouse_dec       +startuptime     -xterm_clipboard
```

Rinstall vim as vim-gnome:   
```
sudo apt-get install vim-gnome
```
Select what you want using the mouse - then type to copy to clipboard:  
```
"+y
```

To paste to vim from clipboard type:  
```
"+p
```
## Others
* Ex: open the current directory
* set number: show line number
