# Seminyak

Really, really, really ridiculously good looking splash page for Hugo.

## Screenshot

![Screenshot of Seminyak theme for Hugo](https://github.com/comfusion/seminyak/blob/master/images/screenshot.png?raw=true)

## Installation

- Copy theme to your site's themes folder.
- Set `theme = "seminyak"` in your config.
- Make it read good and do other things good too.

## Features

- Set your own background image
- Modify header and message
- Tweak style treatments
- Google Analytics using Hugo's internal template
- Open Graph using Hugo's internal template
- RSS using Hugo's internal template
- Overrides for scripts, favicon and analytics
- Native System Font Stack
- Referrer Policy
- Webmaster Verification

## Customization

### Header and Message

To customize the header and message create a `_index.md` at the root of your site's `/content/` directory. Set the `title` in the front matter to define the header text then use HTML or Markdown below the front matter to define the message. See `exampleSite` for example.

### Style

Seminyak uses [CSS Variables](https://devdocs.io/css/using_css_variables) for customization of basic elements. To start customizing copy the theme's `variables.css` into your `/static/css/` directory and have at it.

### Configuration

Just the basics. Add to your site configuration.

```
googleAnalytics = "UA-123-45" # Optional, enable Google Analytics

[params]
  theme_color = "#fffdc3"; # Optional, theme-color meta tag
  referrer_policy = "same-origin" # Optional, referrer policy meta tag

[params.webmaster]
  google = "" # Optional, Google verification code
  bing = "" # Optional, Bing verification code
  alexa = "" # Optional, Alexa verification code
  yandex = "" # Optional, Yandex verification code
```

### Favicon

To add a favicon add a `favicon.html` file in your site's `partials` folder and drop in a `link` tag with your favicon.

### Scripts

To add some scripts do one or both of the following depending on the type of script you wish to add. For asynchronous scripts create a `scripts-async.html` file in your site's `partials` folder and add async scripts there. For blocking scripts create a `scripts-blocking.html` file in your site's `partials` folder and add any blocking scripts there.

## License

Copyright 2018 Josh Habdas <jhabas@protonmail.com> (https://habd.as)
<br>This work is free. You can redistribute it and/or modify it under the
<br>terms of the Do What The Fuck You Want To Public License, Version 2,
<br>as published by Sam Hocevar. See the COPYING file for more details.
