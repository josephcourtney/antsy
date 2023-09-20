antsy - simple utility for building ANSI escape codes for styling text
 
# features
 - separately color foreground, background, and unerlines
 - supports bold, faint, underline, dunderline (double underline), italic, and strikethrough text styles
 - specify 8-bit colors by name
 - 24 bit color support with RGB values (0-255)
 
# examples:
```sh
$> echo "$(antsy -s bold -fg red -bg white) bumfuzzled $(antsy -r)"
[31;107mbumfuzzled[0m
```

```sh
$> echo "$(antsy -rgb -s "italic dunderline" -fg 255 0 255) Hullaballoo $(antsy -r)"
[21;3;38;2;255;0;255mHullaballoo[0m
```
