`<audio>`
- `controls` -> to show play, mute, playback speed
- `autoplay` -> automatically play the audio
- `loop` -> continuously play the audio; **Not recommended**
- you can give the fallback type/format also

```html
<body>
    <p>sample audio</p>
    <audio controls autoplay loop>
        <source src="music/sample_audio.mp3" type="audio/mpeg">
        <source src="music/sample_audio.wav" type="audio/wav"> <!-- backup -->
    </audio>
</body>
```

<br>
<hr>


`<video>`
- supported formats mp4, webm, ogg
- like audio it supports controls, autoplay, 
- also supports muted
- you can keep backup formats also
- you can keep the `<a href>` attribute too

```html
<video src="music/rainy_day.mp4" width="500px" controls autoplay></video>
```