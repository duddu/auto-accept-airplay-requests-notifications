# (Auto) Accept AirPlay Requests

<img src="https://github.com/duddu/auto-accept-airplay-requests/blob/latest/Docs/airplay-notification.png?raw=true" align="right">

This is a lightweight, single-purpose macOS app that automatically allows other devices to AirPlay to your computer, eliminating the need for manual intervention—otherwise required when the device is signed into a different iCloud account.  
It intercepts incoming notifications alerts about devices attempting to AirPlay to your computer and programmatically accepts them.

## Highlights

- Extremely minimal footprint and resource consumption
- Executes only local Swift code, no network requests
- Runs as a low-priority background process
- Starts at login (includes Launch Agent registration)
- Gracefully handles security permissions (and lack thereof)

## Install

This app is a fully self-enclosed bundle, it doesn't install any support files or external resources.

- Download the [latest release](https://github.com/duddu/auto-accept-airplay-requests/releases/latest)
- Extract the app anywhere on your Mac
- Launch it and follow the prompt for permissions

The app is now up and running in the background, and will only make itself visible if anything changes in terms of permissions.

## Who is it for

Anyone wishing to use more than once a macOS machine as an AirPlay receiver/speaker from a device not logged into the same exact iCloud account; especially if they cannot always promptly react to incoming notifications on that machine.  
E.g. you got a mac at home you use as media server, you just want anybody on your network to be able to AirPlay to it from their device. Sounds easy? Right! Sadly, this will never happen without your manual intervention: unless the same iCloud account is logged in on both device and receiver, you'll keep having to manually click "Accept" on the AirPlay request notification. Even if you are on the same network, even if you previously approved the same device, and even if the device user is in your same iCloud Family. And yes, it doesn't matter which option you chose in "Allow AirPlay for" settings (that only determines which devices will be able to *detect* your mac as a receiver).
