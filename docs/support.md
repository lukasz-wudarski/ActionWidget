# ActionWidget Support

Questions, problems or ideas? Email lukasz.wudarski@protonmail.com and include your iPhone model, iOS version, and what you tapped and what happened. Please leave out passwords and tokens.

## Getting started

1. **Set up a button.** Open ActionWidget, tap Widget 1, then a button. Enter the address the button should call, choose the method and add anything else the request needs. Tap Send Test Request to try it.
2. **Add the widget.** Touch and hold an empty spot on the Home Screen, tap Edit > Add Widget, search for ActionWidget and add Widget 1 or Widget 2.
3. **Tap a button.** It shows a spinner while the request runs, then a checkmark when it worked or a cross when it didn't.

## CarPlay

With iOS 26, your widgets also work in CarPlay. On your iPhone, open Settings > General > CarPlay, choose your car, then Widgets, and add ActionWidget's widgets. On cars with a touchscreen, you can tap the buttons right on the car's display. The buttons run in the background, so your iPhone can stay locked.

## More widgets

Tap + in the app to add a widget. To show it, add **Any Widget** to the Home Screen, touch and hold it, tap Edit Widget and choose your widget. In CarPlay settings, tap ⓘ next to Any Widget instead. To remove a widget you added, swipe left on it in the app. Widget 1 and Widget 2 always stay.

## Common questions

**The button shows a cross.** The request failed or returned a status that doesn't count as success. Open the button in the app and tap Send Test Request: it shows the status or the error. By default, statuses from 200 to 299 count as success; you can change this under Response.

**A device on my home network doesn't respond.** Send a test request from the app first, so iOS can ask for permission to reach your local network. You can check it in Settings > Privacy & Security > Local Network.

**"The certificate for this server is invalid."** The device uses its own (self-signed) certificate. If you trust the device, turn on Allow Self-Signed Certificate for that button.

**The server asks for a user name and password.** Enter them under Authentication. Basic and Digest (MD5 or SHA-256) are supported. For token sign-in, add an Authorization header instead.

**Tapping a button opens the app instead.** The button isn't set up yet: it needs a full address starting with http:// or https://, and any problem shown in the app fixed.

**My changes don't show in the widget.** Widgets update when you leave the app, so go back to the Home Screen.

**Does it work while my iPhone is locked?** Yes, once you've unlocked it after the last restart.

**Can a button show a picture?** Yes. If a successful response is an image, such as a camera snapshot, it appears behind the checkmark for a few seconds. SVG images aren't supported.

## Privacy

ActionWidget collects no data. See the [Privacy Policy](https://lukasz-wudarski.github.io/ActionWidget/).

ActionWidget requires iOS 26.
