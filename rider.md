# JetBrains Rider

## Issues

### Window Tiling managers like bspwm, dwm, etc.

Rider doesn't play nice with window tiling managers due to how Java GUIs do some weird parenting logic under the hood. Can be fixed by adding the following lines to a new file under /ect/profile.d/<filename>.sh

```bash
export _JAVA_AWT_WM_NONREPARENTING=1
```

