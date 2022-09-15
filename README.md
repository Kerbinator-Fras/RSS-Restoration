# RSS-Restoration
Restore KSP-RSS to J2000 Eclieptic = 0 to make Solar System not "tilted", and opt for non-principia 2-body users.<br>
Very highly recommended since original RSS is faulty in orbital elements - (1)deceive us about the satellites of gas giants, using inclination relative to planet equator instead of ICRF (Earth equator based, original RSS's main axes). Affecting all satelites of Saturn~Pluto (except Titan). (2)2-body RSS does not consider the System barycenter of planet-moon system, but uses the body center, causing large errors, for example, eccentricity of Earth's solar orbit (0.01609, correct 0.0167). (3)RSS uses the single day data of January 1, 1950. No averaging of any method has been done (maybe the author just didn't care about it), resulting in relative large error.<br>
This is mainly optimized for ones focusing on interplanetary travel instead of staying in Earth-Moon even Near-Earth space. Loss of Earth tilt is not more important than error of orbital elements, and is no bad for stockalike interplanetary players (2-body is naturally imprecise, for parking orbit just use value for J2000 ecliptic). If you think you must introduce Earth tilt to make Earth launch looks correct, install tiltem - but you need to take a look at 1st note of the warning and probably need to cope the pesky stuff yourself.<br>
For solar planets of 2-body RSS-Restoration, I use multi-laps mean value for osculating orbital elements - for planets, averaging of mean anomaly is by averaging it using current-date orbit period and MNA to transfer to MNA of mid-averaging-total-time .I used 8 laps and around 2922 pts for each Solar planet.<br><br>
Current state: mean orbital elements for main 9 bodies (Mercury to Pluto) has been done (2021/10/31). Version 1 with basic tilts and corrections of satelites' orbit plane (not correct position) has been done.
Since plain excel keplerian 6-element average method is not very useful for satelites which suffer from precession, plus its very small eccentricity, making its argument of periapsis shaking heavily,causing unreliable MNA), I may need to find other solutions based on a better understanding of angle of 3-d vectors. <br>
Note that Ceres is the only 900-km size asteroid in the main belt (Pallas, Hygiea together with Vesta are all 400km-size, others in 1-10 is 200km-size, if include vesta is's no reason not to include other 3, which will make RSS grand tour more incredibly hard).Also, it in much better than Vesta if you look perpendicular to solar system plane, right in the "should-be" SMA between Mars and Jupiter. However, for compatibility with other mods, currently I may not delete Vesta.<br>
Minor edits: Edited orbit map planets color (for example, lighten the color of Mercury, Earth, Venus orbit)<br><br>
Warning for TiltEm:<br>
1st: You need to set Earth's invertRotAltitudeThreshold to 1Mm or so to avoid sudden switch of tilt disrupting your launch! And you SHOULD do this(higher than rocket phase maximum altitude for lanch and launch) for ANY planets you want to land on and launch from!<br>
TiltEm's surface effect is achieved by inverse rotation mechanism, you may need to add invertRotAltitudeThreshold manually in config. Adding TiltZ may cause camera to turn suddenly when you pass invertRotAltitudeThreshold. Tiltem should add a few on-rail frames during inverse rotation toggle, but that's NOT reliable up to now, so you NEED to make sure you are always on-rail at the threshold you set.<br>
Anyway: take the risk yourself.
