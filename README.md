# RSS-Restoration
Restore KSP-RSS to J2000 Eclieptic = 0 to make Solar System not "tilted". For non-Principia users, Tilt'Em MUST be installed.
For 2-body version of RSS-Restoration, there is a multi-laps mean value for osculating orbital elements.
I used 8 laps and around 2922 pts for each Solar planet.<br>
Warrenty for TiltEm: TiltEm's surface effect can only be achieved when the planet has invertRotAltitudeThreshold in kopernicus cfg.
Thus, I need to manually add inverRotAltitudeThreshold to most bodies, starting from Jupiter for basis test.
Adding TiltZ may cause camera to turn when you are passing inverRotAltitudeThreshold (but sometimes not?) Experimental.<br>
Current state: mean orbital elements for main 9 bodies (Mercury to Pluto) has been done. - 2021/10/31<br>
Version 1 with basic tilts and corrections of satelites' orbit plane (not correct position, since average method is not very useful for satelites which suffer from precession making its argument of periapsis shaking heavily) has been down.
Note tha Ceres fit in much better than Vesta if you look perpendicular to solar system plane, right in the good place between Mars and Jupiter.
And it is much bigger. However, for compatibility with other mods, currently I may not delete Vesta.<br>
Minor edits: Edited orbit map planets color (for example, lighten Mercury, Earth, Venus orbit)
