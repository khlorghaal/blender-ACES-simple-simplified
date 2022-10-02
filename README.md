![image](https://user-images.githubusercontent.com/6794830/177892064-7e62f019-39c4-4de4-861e-d90a5945621c.png)  
Adds a single [ color management/view transform ] option for ACES colorspace alongside standard and filmic.  
Does not modify or alter existing colorspaces. Only Adds ACES.RGBmonitor_100nits_dim and nothing else.  
Unlike the 500mb "simplified" mod, this takes advantage of blender's reference colorspace being already linear ACES2065-1  
so any conversion-type colorspaces for textures and all that mess is unnecessary.  

**install**  
add these files to your blender install /datafiles/colormanagement  
for windows this is %appdata%\Roaming\Blender Foundation\Blender\[version]\datafiles\colormanagement  
backing up the original folder is also recommended if you dont want to reinstall if things go wrong  

updating blender (on pacman, idk about windows, i use arch btw) will overwrite the ocio config file, but will not delete any new files  
recommend saving a .bak of the ocio file, for easy replacement with each update.  
hopefully this gets PRed before too many people have to do this manually.  

the LUT files were stolen from magic-mark.com but i dont believe licenses (if there even was one) apply to raw data based on a spec
