# Script

## Resize video
```
ffmpeg -i input.mp4  -vcodec libx265 -crf 28 output.mp4
```

## Rotate a video
| Integer | String      | Value                                            |
| ------- | ----------- | ------------------------------------------------ |
|    0    | cclock_flip	| 90° counterclockwise and vertical flip (default) |
|    1    | clock       | 90° clockwise                                    |
|    2    | cclock      | 90° counterclockwise                             |
|    3    |	clock_flip  | 90° clockwise and vertical clock_flip            |

```
ffmpeg -i input.mp4 -vf "transpose=2" -crf 23 -c:a copy output.mp4
```
