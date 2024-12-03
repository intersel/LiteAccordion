# LiteAccordion
LiteAccordion is a horizontal accordion plugin for jQuery. 

## Options
These are the default settings for the liteAccordion plugin:
```
containerWidth : 960,                   // fixed (px)
containerHeight : 320,                  // fixed (px)
headerWidth: 48,                        // fixed (px)

activateOn : 'click',                   // click or mouseover
firstSlide : 1,                         // displays slide (n) on page load
slideSpeed : 800,                       // slide animation speed
onTriggerSlide : function() {},         // callback on slide activate
onSlideAnimComplete : function() {},    // callback on slide anim complete

autoPlay : false,                       // automatically cycle through slides
pauseOnHover : false,                   // pause on hover
cycleSpeed : 6000,                      // time between slide cycles
easing : 'swing',                       // custom easing function

theme : 'basic',                        // basic, dark, light, or stitch
rounded : false,                        // square or rounded corners
enumerateSlides : false,                // put numbers on slides
linkable : false                        // link slides via hash
responsive: {
            maxWidth:0,//width size under that we consider we have to apply these parameters
            //any liteaccordion data
        }
```

## Methods

These are the methods for the liteAccordion plugin:

```
play					// trigger autoPlay on a stopped accordion
stop					// stop an accordion playing
next					// trigger the next slide
prev					// trigger the previous slide
destroy					// remove the accordion, destroying all event handlers and styles (unstyled html content will remain)
debug					// returns a debug object
```

All of these methods are chainable (i.e. they return the original DOM object) with the exception of the debug method.  To call a method, use:

```
$('#yourdiv').liteAccordion('play');
```

To chain methods:

```
$('#yourdiv').liteAccordion('next').liteAccordion('next');
```

## Changelog

**v2.3** - 03/12/2024 - E.Podvin - Intersel
- add 'update' method
- add 'responsive' behaviour
- add https://github.com/nikki/LiteAccordion/pull/78
- add https://github.com/nikki/LiteAccordion/pull/71

**v2.2** - 21/01/2013
 - removed responsive option
 - removed autoScale images option
 - fixed issue #66
 - fixed minor css bugs (ie10)

