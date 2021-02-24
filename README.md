A collection of sample Pokémon encounters from Pokémon Sword and Shield.

# Contents and File Counts
* **Egg**: 30885
* **Encounter Slots**:
    * Fishing - Route 2: 39343
    * Overworld - Route 1 (Captured Wooloo): 63324
    * Overworld - Glimwood Tangle (SH ENG): 5524
    * Overworld - Glimwood Tangle (SH KOR): 46522
    * Overworld - Glimwood Tangle (SW): 205244
    * Overworld - Old Cemetery: 1010
    * Overworld - Slumbering Weald: 6067
    * Tree - Stepping-Stone Sea: 7509
* **Encounter Static**:
    * Gift: Given to you by an NPC. Has your OT.
        * Gmax Bulbasaur: 57
        * Gmax Charmander: 339
        * Gmax Squirtle: 8
        * Porygon: 361
        * Dracozolt: 8612
        * Arctozolt: 1376
        * Dracovish: 395
        * Arctovish: 1747
        * Kubfu: 2409
    * In-Game Trade: Traded to you by an NPC. Has their OT.
        * Regina's Meowth: 998
        * Regina's Ponyta: 8930
        * Regina's Farfetch'd: 512
        * Regina's Alolan Exeggutor: 568
        * Regina's Alolan Marowak: 758
        * Regina's Weezing: 3003
        * Regina's Mr. Mime: 1620
        * Regina's Corsola: 5329
        * Regina's Zigzagoon: 622
        * Regina's Darumaka: 1270
        * Regina's Stunfisk: 1138
        * Romeo's Hattena: 13
    * Overworld: Pokémon that spawn on the overworld where you can bump into them.
        * Lapras (Route 2): 3
        * Galarian Articuno: 1030
        * Galarian Zapdos: 5995
        * Galarian Moltres: 8759
        * Crawdaunt (Turffield): 10
        * Glalie (Route 9): 2
        * Spheal (Frigid Sea): 1631
        * Luxray (Soothing Wetlands): 7092
        * East Gastrodon (Galar Mine No. 2): 14
        * Spiritomb: 7678
        * Abomasnow (Route 10): 3
        * Crustle (Route 8): 11
        * Beartic (Route 10): 4
        * Cryogonal (Snowslide Slope): 216
        * Galarian Stunfisk (Galar Mine No. 2): 104
        * Galarian Stunfisk (Slumbering Weald): 5
        * Volcarona (Loop Lagoon): 1186
        * Cobalion: 3729
        * Terrakion: 26824
        * Virizion: 1829
        * Corvisquire (Route 3): 9
        * Corviknight (Hammerlocke Hills): 3159
        * Eldegoss (Route 5): 6702
        * Chewtle (Route 2): 10
        * Drednaw (Galar Mine No. 2): 15
        * Yamper (Route 2): 4
        * Carkol (Galar Mine): 716
        * Obstagoon (Route 2): 26
        * Falinks (Route 8): 23
    * Scripted: Pokémon that require you to interact to start an encounter.
        * Regirock: 10490
        * Regice: 13327
        * Registeel: 2764
        * Regigigas: 3777
        * Impidimp (Glimwood Tangle): 15597
        * Morgrem (Glimwood Tangle): 34
        * Zacian: 15412
        * Zacian (Shiny Enabled): 20174
        * Eternatus: 1536
        * Regieleki: 4709
        * Regidrago: 149
        * Calyrex: 3807
* **Mystery Gift**: Collected from official servers by a hard-working bot.
    * KIBO Pikachu: 756
    * Original Cap Pikachu: 645
	* Hoenn Cap Pikachu: 641
	* Sinnoh Cap Pikachu: 637
	* Unova Cap Pikachu: 635
	* Kalos Cap Pikachu: 633
	* Alola Cap Pikachu: 656
	* Partner Cap Pikachu: 640
	* World Cap Pikachu: 647
    * VGC20 Porygon2: 1328
* **Raid**: 20312
* **Restricted Sparring**: Dumped opponent Pokémon from the IoA Restricted Sparring challenge. 801

# FAQ

### How did you get these files?  
These were all dumped directly from the game using CFW.

### How legitimate are these files?  
For the purposes of data analysis, all of these are unmodified files dumped from an unmodified stock game except for the following:  
* The shiny Zacian directory used a ROM edit to remove the shiny lock.
* Any Pokémon with the Original Trainer name "Redact" was obtained from another user and the OT was changed to maintain their privacy.

### Why are some files missing met location and trainer data?  
Many wild encounters are dumped from RAM and the Pokémon was never captured to save time. This still allows for analysis of all other traits except for a few which are generated after capture.

### Can I trade them in legitimate trading communities?  
Complete Pokémon should be considered clones. Partial Pokémon require further editing which immediately makes them illegitimate. Whether anything here is safe to trade depends on your specific community's rules. Please be considerate and check before trading anything from here as legitimate.

### Can I use these files?  
Yes. As above, please be responsible with them if you plan to trade them to others.

### Can I contribute files?  
I prefer to keep this limited to my own files since I know how they were obtained, but we can discuss if you have something interesting.

### Can I request a particular encounter to be added?  
Yes, as long as it's easy to automate sampling.

### How do I download only specific folders and not the entire repository?  
There are many ways to do this. I manage this locally using git command line tools for sparse checkouts.  As an example:  
```
git clone --filter=blob:none --sparse https://github.com/Lusamine/Anubirb.git
git sparse-checkout init
git sparse-checkout set <directory1> <directory2>
```
For example, `git sparse-checkout set "Mystery Gift/025-04 Unova Cap Pikachu"` will get the entire folder of Unova Cap Pikachu and nothing else. Changing what you have set will erase files that are no longer set and download any new ones.
