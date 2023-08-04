# Ad-Blocker
Extensions are software programs built on web technologies (such as HTML, CSS, and JavaScript) that enable users to customize the Chrome browsing experience.
Making extensions is quite interesting and also simple.
Every extension requires a JSON-formatted file, named manifest.json, that provides important information. This file must be located in the extension's root directory.
The following code shows the supported manifest keys.
{
  // Required
  "manifest_version": 3,
  "name": "My Extension",
  "version": "1.0.1",

  // Recommended
  "action": {...},
  "default_locale": "en",
  "description": "A plain text description",
  "icons": {...},

  // Optional
  "author": "developer@example.com"


  
