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
}

Some of the descriptions of things used in my extension

The chrome.declarativeNetRequest API is used to block or modify network requests by specifying declarative rules. This lets extensions modify network requests without intercepting them and viewing their content, thus providing more privacy.

Rules are specified in JSON files referenced under the "rule_resources" manifest key.
Each file should contain an array of rules as in the example.
A single declarative Rule consists of four fields: id, priority, condition, and action. There are the following kinds of rules:

Rules that block a network request.
Rules that prevent a request from getting blocked by negating any matching blocked rules.
Rules that redirect a network request.
Rules that modify headers from a network request.


