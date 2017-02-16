## Classic patterned bitmap tiled wallpapers

#### Recognition goes to [Anthony Thyssen](http://www.ict.griffith.edu.au/anthony/icons/) for maintaining these bitmaps for 25 years. These images (and more) are for now also available on his old page.

#### Hero
The hero folder comes from [Hero Pattern](http://www.heropatterns.com/) made by Steve Schoger. Note that the quality isn't uniformly great because they were simply converted from svg files by imagemagick.

###### Rediscovered by /u/bdrum in [this reddit post](https://www.reddit.com/r/unixporn/comments/5o29pt/found_a_bunch_of_bitmaps_for_xsetroot_wallpapers/)

#### Creating a repo to help preserve the find

Set with xsetroot. Examples:  
 - Simple example  
`xsetroot -bitmap [selection].xbm`  
 - Add colors  
`xsetroot -bitmap [selection].xbm -bg "color" -fg "color"`  
 - Leverage current colors from xrdb  
`xsetroot -bitmap [selection].xbm "$(xrdb -query|awk '/\*color8:/ {print $2})" -fg "$(xrdb -query|awk '/\*color7:/ {print $2}')"`  

##### Pattern Previews

![preview](preview.png)

