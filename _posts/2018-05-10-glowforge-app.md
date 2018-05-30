# Glowforge app for macOS

So I found out about [nativefier](https://github.com/jiahaog/nativefier) and used it to create a "native application" for the Glowforge. 
Okay, it's really just a customized browser that is only good for the app.glowforge.com website,
but it does give me an actual Glowforge icon in my tray so I don't need to start Chrome and then
go to app.glowforge.com anymore. I suppose that's worth a few megabytes...

Here's how I made it:

```
nativefier --name "Glowforge" --icon icon.png --single-instance --fast-quit https://app.glowforge.com/
```

Here's the icon file:

![icon](/assets/icon.png)

Of course it is also possible to create a Windows app (or even a Linux app) too...

There are probably some other interesting possibilites too. For example:

I should play with some of the options to disable the browser's debugger and context menu in order to simplify the UI. (I think I want to keep the clipboard commands though.)

Rather that going right to app.glowforge.com, the app could maybe load a local page (part of the app itself) which adds a material manager and then starts the normal glowforge page. (Nativefier also has an "inject" command which can be used to add Javascript code to each page...)

Maybe include a toolbar or menu options that show box and other shape generators in the app?
