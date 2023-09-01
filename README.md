# BlackShades

A fork of Black Shades that is updated to build on Linux. Original game was created by Wolfire games - http://www.wolfire.com

Orignal was coded by David Rosen. Using source from https://www.icculus.org/blackshades

## Gameplay
Try to keep your VIP (the guy in white) alive as long as possible. The assassins will all try to shoot or stab him to death. You must do all you can to prevent this. Your reputation has preceded you, so the VIP has absolute confidence in your abilities and will completely ignore all the assassins. When an assassin is aiming at your VIP with a gun, you will psychicly see a line of sight extending from him to your VIP. This line will narrow and redden until it disappears and the assassin fires. Depending on the situation it may be best just to shoot the assassin(s), or to dive and tackle the VIP to the ground to avoid the bullet. Unfortunately your psychic powers do not show the line of sight of knife-wielding assassins.

If you are feeling overwhelmed you can use psychic aiming to temporarily speed up your thought processes and aim your shots better. If there are no visible enemies you may want to release your soul and look for nearby enemies. When your soul is released your VIP pulsates between blue and red, civilians between black and red, and assassins are solid red.

If you die or your VIP is killed.. the level restarts. If you are are interested in the theory behind this: you are a psychic bodyguard, so you can see small distances into the future. The failure only occured in a possible future which you are now going to try and avoid.

You can edit levels by setting "Custom levels" to 1 in the config and editing the customlevels.txt file in the data folder.

### Controls
<ul>
<li>WASD = walk</li>
<li>shift = run</li>
<li>mouse = look</li>
<li>control = crouch/zoom</li>
<li>click = fire (while aiming) or smash (while running) or pick up gun (while crouching over a body and not aiming) or disarm (while not aiming)</li>
<li>q = aim or un-aim (important for picking up guns)</li>
<li>r = reload</li>
<li>e = psychic aim</li>
<li>z = toggle soul release</li>
<li>space = dive (while running forwards)</li>
</ul>

keys for debug mode:

<ul>
 <li>tab = 3rdperson toggle </li>
 <li>f = Force Push </li>
 <li>shift-x = switch weapons </li>
</ul>

### Scoring
The scoring system consists of:
<ul>
<li>150 points for a successful disarm</li>
<li>300 points for destroying a zombie (by blowing its head off) </li>
<li>100+50x points for completing a mission where x is the mission number (i.e. 450 points for completing mission 3) </li>
<li>75 points for incapacitating an assassin </li>
     <ul>
     <li>+50 if he had a knife</li>
     </ul>
<li>-300 points for hurting a civilian </li>
<li>-200 points for allowing the VIP to die </li>
</ul>

The penalty for failing to protect the VIP is halved if you kill the assassin.

### Weapons:
<ul>
<li>Bare Hands: Smack people with them. Or if you want to be nice, walk or stand (don't run) near somebody with a gun and take it away.</li>

<li>Knife: Like bare hands, but deadly and with longer range. Look out for knife-wielding assassins, they are the most dangerous.</li>

<li>Handgun: One shot with this should be enough to incapacitate any human target, but they may remain conscious for a second (this can be bad if they are about to stab your VIP, aim for the head)</li>

<li>Magnum:  Not as much ammo as the vanilla handgun, but one shot is an instantenous kill</li>

<li>Assault Rifle: This weapon has quite a kick and is bigger and more unwieldy than the handguns, but it has a large magazine and can fire quickly if necessary</li>

<li>Sniper Rifle: A bit more powerful than the magnum, with a scope. Very difficult to aim unless you are zoomed in (zoom by holding the control key)</li>

<li>Shotgun: Aim and shoot. Very powerful but somewhat inaccurate.</li>

<li>Grenade: Hold down the mouse button to take out the pin, release the button to throw it. Crouch to change your mind and put
the pin back in. You can knock people out if you hit them in the head, or  of course you can just blow them to pieces.</li>
</ul>

## Building
Currently, source has been tested to build on Unix-like systems. No testing done on Mac or Windows.

### Requirements

<ul>
  <li>SDL</li>
  <li>SDL_image</li>
  <li>freealut</li>
  <li>freeglut</li>
  <li>OpenAL</li>
  <li>libogg (optinal)</li>
  <li>libvorbis</li>
</ul>

### Compile & Run

Currently, compiling with clang produces no errors, but not with GCC.

Building on Linux with clang will be the default until GCC is supported.

Compile in root directory:

```
make 
```

Run game:

```
./objs/blackshades
```


## Notes from original source tree
<ul>
<li>Main menu music is included with permission from musician John Graham, Copyright 2002.</li>
<li>Due to legal difficulties all other music is composed by me at the last minute based on some nice loops made by Carlos Camacho, hence the 'programmer music'.</li>
<li>Also many thanks to my other friends and beta testers, and to artist David Drew for modelling the assault rifle, sniper rifle, handgun, shotgun and grenade.</li>
</ul>

Known bugs for orignal code:
<ul>
  <li>It doesn't work too well under classic emulation</li>
  <li>Occasional collision detection issues</li>
  <li>Turning virtual memory off can cause speed issues</li>
</ul>
