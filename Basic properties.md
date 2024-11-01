# The basics

------

### Stats

First step of creating any battle is to change image and basic properties of the enemy. It's actually very simple.
 First, go to the **g.engine** sprite. It sets all the stats, both for the player and for the monster. Then, look on this script:
![g_engine](https://ltnlittlecoder.github.io/g_engine.jpg)
 A lot of stuff, right? But it's not that complicated. Different sections are separated by **"hide"** blocks for convience.



**Monster** sections sets monster's stats.


 -**g.mon_hp** is monster's HP at the beggining of the battle. In case of Froggit it's 30. Should not be higher than **max HP**, or the hp bar will act strange.
 -**g.mon_hp.max** is monster's max HP. *It's recomended to set it the same as **g.mon_hp***.
 -**g.mon_spareable** defines if monster can be spared from the start or not. **0** means no, **1** means yes.
 -**g.mon_def** is monster's DEF (defense) stat.
 -**g.mon_att** is monster's AT (attack) stat.



**Player** sections sets player's stats.

-**g.pl_att** sets player attack. See [stats chart on Undertale Wikia](http://undertale.wikia.com/wiki/Stats) for more info.
 -**g.pl_wp.att** sets player weapon's attack. See [ items list on Undertale Wikia](http://undertale.wikia.com/wiki/Category:Items) for more info.
 -**g.pl_def** sets player's DEF. See [stats chart on Undertale Wikia](http://undertale.wikia.com/wiki/Stats) for more info.
 -**g.pl_hp** sets player's HP. Should not be higher than 99, or HP bar will glitch. 
 -**g.pl_hp.max** sets player's max HP. Should not be higher than 99, or HP bar will glitch. See [stats chart on Undertale Wikia](http://undertale.wikia.com/wiki/Stats) for more info.



**ACT menu** section adds stuff to ACT menu! There can be 4 elements at once. Refer to [ text engine tutorial](https://ltnlittlecoder.github.io/Text Engine) for explaination of what to type.



**Items** section adds stuff to ITEM menu! There can be 4 elements at once. Refer to [ item list](https://ltnlittlecoder.github.io/items.html) for list of useable items.



**Messages** section sets displayed messages!

You should know how [text engine](https://ltnlittlecoder.github.io/Text Engine) works by now.
 -**text.win** is text displayed after you kill enemy.
 -**text.spare** is text displayed after you spare the enemy.
 -**text.flee** is text displayed when you try to run away.
 -**text.encounter** is text that is displayed in the main menu.
 -**text.check** is text displayed when you use CHECK from the ACT menu.
 -**text.act1, text.act2, text.act3** are displayed when you choose something from the act menu, I don't think I have to explain them.
 -**text.mon_text_bubble** is thing that enemy says before attacking. IT DOES NOT USE THE TEXT ENGINE. YOU JUST TYPE AS NORMAL.



###  Changing enemy image

Just delete all of the costumes of **g_monster** sprite and replace them with new ones. They will be animated by default.
![costumes](https://ltnlittlecoder.github.io/costumes.jpg)
 Change this script to modify animation speed or stuff like that. **Wait 0 secs** is there to slow down animation by one frame per second.

**So, those are the basics. You can already create something with it,  but you probably want to make your own attacks, and set what ACTing  does, right?
 [Well. You can learn it in part 2, here!](https://web.archive.org/web/20200202183812/http://scratchtale.orgfree.com/tut2.html)**
