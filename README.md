A collection of sample Pokémon encounters from Pokémon Sword and Shield.

# Contents and Counts
See the [Wiki](https://github.com/Lusamine/Anubirb/wiki) for a full list of all Pokémon uploaded to this repository.

# FAQ

### How did you get these files?  
These were all dumped directly from the game using CFW.

### How legitimate are these files?  
For the purpose of data analysis, all of these are unmodified files dumped from an unmodified stock game except for the following:  
* The shiny Zacian directory used a ROM edit to remove the shiny lock.
* HOMEbound Pokémon from Pokémon GO were dumped from HOME as they cannot be moved into Sword/Shield.
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

### How do I search for specific files to download?  
Look at this repository on GitHub web and type "t". It should activate the file finder. You should be able to search by species, nature, IVs, OT, TID, ball, and the checksum-EC string. This make take a few seconds since there are many files.  
![image](https://user-images.githubusercontent.com/30205550/109421984-39b73100-799f-11eb-84bf-17d1cb4c2e15.png)

If this doesn't work for you, you can use the [Advanced Search](https://github.com/search/advanced?q=repo%3ALusamine%2FAnubirb&type=Code) and enter your search in "Code options > With this file name".

### How do I download a specific folder and not the entire repository?  
There are many ways to do this. I manage this locally using git command line tools for sparse checkouts.  As an example:  
```
git clone --filter=blob:none --sparse https://github.com/Lusamine/Anubirb.git
git sparse-checkout init
git sparse-checkout set <directory1> <directory2>
```
For example, `git sparse-checkout set "Mystery Gift/025-04 Unova Cap Pikachu"` will get the entire folder of Unova Cap Pikachu and nothing else. Changing what you have set will erase files that are no longer set and download any new ones.
