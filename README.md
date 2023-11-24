# Unlimited-Quest-Storage

The limited storage space of the base Quest models have been an issue for some time. Fortunately, there is a way to save storage without uninstalling games.

## The Idea
The Quest, while it doesn't have an SD card port, does have a USB-C port with data. This can be used to transfer data on and off the Quest, possibly even using the Quest itself. The idea is to transfer games off the Quest and onto an external storage device (i.e. USB drive, external HDD, SD card).

### Unlimited?
Currently, no. The goal is for this project is to eventually become "unlimited", where the only limits are your external storage. 

## Steps
**DISCLAIMER: THIS HAS NOT BEEN WIDELY TESTED.** As of writing this, I have only tested one app, which only had files in `/Android/data` and none in `/Android/obb`. I am not responsible for losing game progress or damaging your system.

To achieve storage reduction, you must either 1. sideload a file manager or 2. have another device, capable of connecting and acting as such (phone, laptop, etc.). Once you've connected, go to `/Android` and copy over `/Android/data/[app]` and `/Android/data/obb` to your external storage. Note that not all apps may have data or extra assets. In that case, there isn't any extra data you can reduce without uninstalling the app. Once you have copied over the data, delete the folders off the Quest.

**I do not know how an app will react after this.** I recommend not launching any app after extracting the data until you restore it. 

**Restoring:**
To restore, simply do the opposite. Copy the data from your external storage over to the Quest in the same area you took it from. Once you do so, the app should run like it was.

### How Much Does This Save?
This depends on the apps you have installed. On my system with 150gb of apps, I can save around 90-95gb of storage.

## The Future
Hopefully, we will find a way to extract the entire app from the system. This way, we would have "unlimited" data, and wouldn't have to worry about accidently starting a "disabled" app.

### I Need Help!
I am not an app developer. I have some experience with programming, but not enough to make an app that does this. If somebody could help me create a *native* Quest app that would automatically load and unload games, it would be an amazing tool for the community.
