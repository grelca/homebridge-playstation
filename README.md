<p align="center">

<img src="https://github.com/homebridge/branding/raw/master/logos/homebridge-wordmark-logo-vertical.png" width="150">

</p>

# Homebridge Playstation

### Playstation integration for Homebridge / HOOBS.

_Hey Siri, turn on Playstation_ finally possible!

This integration exposes a Switch service that can be used to switch on/off your PS4/PS5, and determine its current state.

Most of the work is done by the amazing [playactor](https://github.com/dhleong/playactor) library, which this project depends on.

## Installation

You can install it via Homebridge UI or manually using:

```bash
npm -g install homebridge-playstation
```

## Configuration

Before doing anything, switch on your PlayStation.

Now you need to configure **PlayActor** and follow the authentication process provided by the library; to do so, open the Homebridge Terminal and run:

```bash
homebridge-playstation-login
```

Open the authorization link provided, authenticate it using your PSN account, and copy the URL when the page shows "redirect" in the terminal.

Once you've done that, go to Settings > System > Remote Play > Link Device and provide the PIN code.

Cool, now just restart the HomeBridge instance, and your PlayStation should be visible in the Home app.

## Parameters

- `pollInterval`: Determine how often should informations be fetched (in milliseconds)
