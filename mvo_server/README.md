## Overview
A recreation of the Previous Microvolts reward systems, bringing back the achievement and reward mechanics from Microvolts Unplugged and ToyHeroes Offline. 

```
    |  \/  | \ \ / /  / _ \  
    | |\/| |  \ V /  | (_) | 
    |_|__|_|  _\_/_   \___/  
    _|"""""|_| """"|_|"""""| 
    `-0-0-'  `-0-0-'  `-0-0-` 
    
MVO v0.5
──────────────────────────────────────────────────────────────
```
## Project Status
I’m no longer actively working on this project. My interests have shifted toward reverse engineering, exploit development, and studying offensive security, mainly focusing on C++ and Rust. Because of that, I haven’t had the time or motivation to keep this repo maintained

If you’d like to continue the work or take it in your own direction, feel free to fork it.

## Features
- Referral Wheel
- Event Shop
- Achievement system
- daily playtime chest

### Achievement GUI Status
This project is implemented in vanilla JavaScript and was mainly intended as a backend system. I couldn’t get the web interface for the achievements to look right. CSS scaling is off and it’s not responsive. it can be used for testing backend functionality.
![Current Achievements GUI State](docs/achievements-buggy.png)


### Achievements Progression
The original setup rewarded MP, Battery, Coins, and a few special items unlocked after reaching level 90. However, progression relied heavily on farming, which made it feel overly grindy. The current setup still rewards the same currencies but also introduces RT, coupons, and WC variants for levels 50 and above. Try to keep a good balance so players do not get items too early or too late.

You will need to manually edit the `generateAchievements.js` script located at `util/scripts/generateAchievements.js`. The script is simple enough to modify, so customizing the rewards should not be difficult.


Integration with the [MicrovoltsEmulator](https://github.com/SoWeBegin/MicrovoltsEmulator) is already in place, so achievements can directly trigger reward delivery to players. You can test the server endpoints with Postman to verify that achievements and reward calls work correctly.


### Installation & Configuration

check out [Installation & Configuration](docs/configuration.md)


### Note
Parts of this documentation were originally generated and may contain duplicated or inconsistently formatted sections. For accuracy, cross-reference with the source code.



