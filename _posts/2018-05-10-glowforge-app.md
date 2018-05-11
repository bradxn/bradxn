# Glowforge app for macOS

So I found out about [nativefier](https://github.com/jiahaog/nativefier) and used it to create a "native application" for the Glowforge. 
Okay, it's really just a customized browser that is only good for the app.glowforge.com website,
but it does give me an actual Glowforge icon in my tray so I don't need to start Chrome and then
go to app.glowforge.com anymore. I suppose that's worth a few megabytes...

Here's how I made it:

```
nativefier --name "Glowforge" --icon icon.png --single-instance --fast-quit https://app.glowforge.com/
```
