#WaveLoading Xamarin Binding

This library provides a *wave loading* animation as a **Drawable**.

![screenshot](./screenshots/screenshot.gif)

## How to use

Add Reference to the project and include the namespace
```
using Com.Race604.Drawable.Wave;
```

Use in your project with only one line:

```
Drawable mWaveDrawable = new WaveDrawable(otherDrawable);

// Use as common drawable
imageView.SetImageDrawable(mWaveDrawable);
```


Other configurable APIs:
```
public void setWaveAmplitude(int amplitude), set wave amplitude (in pixels)

public void setWaveLength(int length), set wave length (in pixels)

public void setWaveSpeed(int step), set wave move speed (in pixels)

public void setIndeterminate(boolean indeterminate), like progress bar, if run in indeterminate mode, it'll increase water level over
and over again, otherwise, you can use boolean setLevel(int level) to set the water level, acting as loading progress.

public void setIndeterminateAnimator(ValueAnimator animator), set you customised animator for wave loading animation in indeterminate mode.
```
Original Java Project
https://github.com/race604/WaveLoading


## License
MIT
