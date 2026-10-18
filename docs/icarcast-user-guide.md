# iCarCast user guide

iCarCast is CarCast for iPhone and iPad. It turns an iPad or an iPhone into a CarPlay screen, and it can run CarPlay
on the iPhone itself. On the home screen the app is called **CarCast**.

![CarCast home screen on iPhone](../screenshots/iphone-home.png)

## What you can do

| Device | Use |
|---|---|
| **iPad** | A CarPlay screen for your iPhone, for example mounted in a car that has no CarPlay. |
| **iPhone** | The same, as a screen for another iPhone. |
| | **This iPhone:** CarPlay on the same iPhone, full screen. |
| | **Connect:** send CarPlay from this iPhone to an iPad (or another iPhone) running CarCast. |

You need iOS or iPadOS 15 or later, and an iPhone with CarPlay enabled (Settings › General › CarPlay).

## Installing

- **TestFlight:** if you were invited, open the invitation on the iPhone or iPad and install **iCarCast** from the
  TestFlight app.
- **Sideloading:** download the `.ipa` from [Releases](https://github.com/rPlayAI/carcast-public/releases) when one is
  posted, and install it with AltStore, SideStore or Sideloadly.

On first launch, allow what CarCast asks for:

- **Local Network**, so the iPhone can find the CarCast screen.
- **Location**, because iOS only tells apps the Wi-Fi network's name when location is allowed.
- **Bluetooth**.

## The home screen

The screen shows this device's car name (`CarCast-XXXX`) and what it is doing, with these buttons:

- **Settings**: car name, logo, display and instrument cluster.
- **Connect** (iPhone): start CarPlay on another CarCast screen.
- **This iPhone** (iPhone): CarPlay on this iPhone.
- **Stop**: replaces Connect or This iPhone while CarPlay is starting or running, and ends it.
- **Back to CarPlay**: appears when you've left CarPlay for CarCast's own screen (below).

## Using an iPad as the CarPlay screen

1. Open CarCast on the iPad. It shows **Waiting for iPhone**.
2. Put the iPhone and the iPad on the same network. In the car, turn on **Personal Hotspot** on the iPhone and join it
   from the iPad.
3. On the iPhone, open CarCast and tap **Connect**, then pick the iPad by its name.

CarPlay appears on the iPad and its sound plays from the iPad. Touch works as on a car screen.

The first time, the iPhone asks **Allow CarPlay While Locked?** That card can't be tapped while CarPlay is on screen;
answer it on the iPhone in Settings › General › CarPlay › `CarCast-XXXX`. You're asked once per CarCast device.

## This iPhone

Tap **This iPhone**. CarPlay fills the iPhone's screen, the way it would look in a car, and sound stays on the iPhone.
Tap **Stop** to end it.

![CarPlay on the same iPhone](../screenshots/iphone-this-iphone-carplay.png)

At home, be on Wi-Fi. In the car, turn on **Personal Hotspot** and keep Wi-Fi on. If CarPlay doesn't appear within
about 10 seconds, CarCast tries once more by itself; if it still doesn't start, tap **This iPhone** again.

## The car icon and Back to CarPlay

The CarPlay home screen has an icon for the car itself (LEXUS until you choose your own logo). Tap it to leave CarPlay
for CarCast's own screen, which says **CarPlay is connected**. Tap **Back to CarPlay** to return, or **Settings** to
change the car.

## Settings

| Car | Display | Instrument cluster |
|---|---|---|
| ![Car settings](../screenshots/iphone-settings-car.png) | ![Display settings](../screenshots/iphone-settings-display.png) | ![Instrument cluster settings](../screenshots/iphone-settings-cluster.png) |

**Car**

- **Car name**: the name the iPhone shows for this car.
- **Car logo**: the car's icon on the CarPlay home screen. Choose a square image; **Remove** goes back to the default.

**Display**

- **Resolution**: *Fit this screen* (this device's own screen size), *Widescreen (1920 × 720)*, *Standard (800 × 480)*
  or *Full HD (1920 × 1080)*.
- **Video playback**: lets apps that support it show video on the CarPlay screen while parked.
- **Show touches**: marks each tap, for screen recordings. Takes effect at once.

**Instrument cluster**

A second CarPlay screen, like the one behind a car's steering wheel, shown beside or under the main screen. It has no
touch input, as in a car.

- **Content**: *Map*, *Turn card* (the next turn) or *Navigation app decides*.
- **Show ETA**: the arrival time on the cluster.
- **Size**: *Small*, *Medium* or *Large*.

**About** shows the version and this device's details, for problem reports.

Most changes are read by the iPhone when it connects, so CarCast offers **Quit CarCast** after a change: open it again
and reconnect for the change to take effect.

## Wi-Fi and networks

Where you are decides what to switch on: at home, the same Wi-Fi for both devices; in the car, the iPhone's Personal
Hotspot, with Wi-Fi on. Wi-Fi must never be switched off. The **[Wi-Fi and network guide](ios-network-guide.md)**
covers every case.

## Open CarCast automatically

iOS doesn't let apps start themselves, but a Shortcuts automation can: Shortcuts › Automation › New › **Charger** (the
iPad on car power) or **Bluetooth** (your car) › action **Open App › CarCast** › **Run Immediately**.

## Troubleshooting

| Problem | Try |
|---|---|
| **No CarCast screen found on this Wi-Fi** | Both devices on the same network; Local Network allowed for CarCast on both; avoid public or hotel Wi-Fi (use the iPhone's hotspot). |
| **CarPlay didn't start** | Check Wi-Fi is on (and Personal Hotspot in the car), then tap the button again. |
| CarPlay worked before, now never starts | Restart the iPhone. |
| A setting didn't change anything | Quit CarCast, open it again and reconnect. |

Still stuck? [Report a problem](https://github.com/rPlayAI/carcast-public/issues/new/choose) with both devices' models
and iOS versions, and what you tried.
