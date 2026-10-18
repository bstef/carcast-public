# CarCast for iPhone and iPad: Wi-Fi and network guide

CarPlay is a wireless connection, so where you are (home, a café, the open road) decides what has to be switched on.
This page covers the three ways to use CarCast on iOS and iPadOS.

| You want | At home or work | In the car / on the road |
|---|---|---|
| **This iPhone**: CarPlay on the same iPhone | Join your Wi-Fi as usual | Turn on **Personal Hotspot**, keep **Wi-Fi on** |
| **An iPad (or second iPhone) as the CarPlay screen** | Both on the same Wi-Fi | iPad joins the **iPhone's Personal Hotspot** |
| **Connect**: send CarPlay from your iPhone to a CarCast screen | Both on the same Wi-Fi | iPad joins the **iPhone's Personal Hotspot** |

Two rules hold everywhere:

- **Wi-Fi must be on.** Not necessarily joined to a network, but the Wi-Fi switch in Settings must be on. With Wi-Fi
  off, iOS never starts CarPlay.
- **Allow the permissions CarCast asks for** on first launch: **Local Network** (the iPhone finds the CarCast screen),
  **Location** (iOS only tells apps the Wi-Fi network's name when location is allowed) and **Bluetooth**.

## This iPhone (CarPlay on the same iPhone)

Tap **This iPhone** on the CarCast home screen. CarPlay fills the screen; sound stays on the iPhone.

| iPhone's network | Result |
|---|---|
| Joined to a Wi-Fi network | ✅ Works |
| Personal Hotspot on (needs mobile data), Wi-Fi on | ✅ Works, including on the open road. **Use this in the car.** |
| Wi-Fi on but not joined, hotspot off | ⚠️ Only near a Wi-Fi network the iPhone already knows; the iPhone may join it on its own. On the open road it won't start: turn on Personal Hotspot. |
| Wi-Fi off | ❌ Doesn't start |

- **Personal Hotspot needs mobile data.** If the switch is greyed out in Settings, your plan or carrier doesn't allow
  it.
- **If no CarPlay screen appears within about 10 seconds,** CarCast tries again once by itself. If it still says
  *CarPlay didn't start*, tap **This iPhone** again.
- **Typing a Wi-Fi name.** If CarCast can't read the network name (location not allowed), it asks for it. Type it
  exactly: a misspelt name makes the iPhone go looking for that network and leave the one it is on.
- **Keep CarCast in front.** Switching to another app can end the session; tap **This iPhone** to start again.

## An iPad as the CarPlay screen

The iPad runs CarCast and shows **Waiting for iPhone**. The iPhone that drives it has to be on the same network:

- **At home:** both on the same Wi-Fi.
- **In the car:** turn on Personal Hotspot on the iPhone and join it from the iPad (Settings › Wi-Fi on the iPad). This
  is how CarCast is used on the road, and the iPad also gets internet through the iPhone.

Then start CarPlay from the iPhone with **Connect** (below).

## Connect (iPhone → another CarCast screen)

1. Put both devices on the same network (see above).
2. Open CarCast on the iPad first, then on the iPhone tap **Connect**.
3. Pick the screen by name (`CarCast-XXXX`, also shown on the iPad's home screen).

If it says **No CarCast screen found on this Wi-Fi**, the two devices can't see each other:

- Check that they really are on the same network (the iPad on the iPhone's hotspot, not on a nearby Wi-Fi).
- Check **Local Network** is allowed for CarCast on both: Settings › Privacy & Security › Local Network.
- **Public, hotel, café and office guest Wi-Fi** usually block devices from seeing each other. Use the iPhone's
  Personal Hotspot instead.

## The first connection

- The iPhone asks **Allow CarPlay While Locked?** for each new car. While CarCast shows CarPlay, that card can't be
  tapped on the same screen; answer it in Settings › General › CarPlay › the car (`CarCast-XXXX`).
- Each iPad or iPhone running CarCast is its own car, and keeps its identity across reinstalls, so you're asked once.

## When nothing works

- **Restart the iPhone.** If CarPlay connected before and now never starts, even on a network that worked, the iPhone's
  CarPlay service is stuck. A restart fixes it; CarCast itself doesn't need resetting.
- **Turn Wi-Fi off and on** on the device running CarCast, then try again.
- Still stuck? [Report a problem](https://github.com/rPlayAI/carcast-public/issues/new/choose) with both devices'
  models and iOS versions and which of the cases above you were in.

## Tip: open CarCast automatically

iOS doesn't let apps start themselves, but a Shortcuts automation can open CarCast when you get in the car: Shortcuts
› Automation › New › **Charger** (the iPad on car power) or **Bluetooth** (your car) › action **Open App › CarCast** ›
**Run Immediately**.
