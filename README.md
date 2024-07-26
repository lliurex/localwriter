# localwriter: A LibreOffice extension for local generative AI

Consider donating to support development: https://ko-fi.com/johnbalis


## About
This is a libreoffice writer extension to allow for inline generative editing with local inference. It can be used with any language model supported by text-generation-webui. 

This extension adds two powerful commands to libreoffice writer:

### Extend Selection
Uses a language model to predict what comes after the selected text. There are a lot of ways to use this.

Some example use cases for this include, writing a story or an email given a particular prompt, adding additional possible items to a grocery list, or summarizing the selected text. 

### Edit Selection
A dialog box appears to prompt the user for instructions about how to edit the selected text, then the selected text is replaced by the edited text. 

Some examples for use cases for this include changing the tone of an email, translating text to a different language, and semantically editing a scene in a story. 

## Setup

First go to tags, and download the most recent version of `localwriter.oxt`. 

In libreoffice, Navigate to Tools, then Extensions Manager, then click `Add` and find the `localwriter.oxt` file in your filesystme. You will be directed to read the license then the extension should be installed.

You will also need to setup `text-generation-webui`, and enable the local openai API (note that this just means in this mode `text-generation-webui` will respond in the same format as open AI, all the computation still happens on your computer!). You can use whatever model you want, but I'd recommend openchat3.5 if you don't have a particular model in mind and have only 8 gigabytes of VRAM. Once the OpenAI-style API is running on localhost port 5000, localwriter should work with no additional steps. 

## Hotkeys

Extend Selection is bound to ctrl + q by default, and Edit Selection is bound to ctrl + e by default. 

## License 

(See License.txt for the full license text)

Except where otherwise noted in source code, this software is provided with a MPL 2.0 license.

The code not released with an MPL2.0 license is released under the following terms.
License: Creative Commons Attribution-ShareAlike 3.0 Unported License,
License: The Document Foundation  https://creativecommons.org/licenses/by-sa/3.0/

A large amount of code is derived from the following MPL2.0 licensed code from the Document Foundation
https://gerrit.libreoffice.org/c/core/+/159938 


MPL2.0

Copyright (c) 2024 John Balis