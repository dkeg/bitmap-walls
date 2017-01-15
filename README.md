## Classic patterned bitmap tiled wallpapers

#### Recognition goes to /u/bdrum from this post (https://www.reddit.com/r/unixporn/comments/5o29pt/found_a_bunch_of_bitmaps_for_xsetroot_wallpapers/)

#### Creating a repo to help preserve the find

Set with xsetroot. Examples:  
 - Simple example  
`xsetroot -bitmap [selection].xbm`  
 - Add colors  
`xsetroot -bitmap [selection].xbm -bg "color" -fg "color"`  
 - Leverage current colors from xrdb  
`xsetroot -bitmap [selection].xbm "$(xrdb -query|awk '/\*color8:/ {print $2})" -fg "$(xrdb -query|awk '/\*color7:/ {print $2}')"`
