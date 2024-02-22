`<audio>`
- `controls` -> to show play, mute, playback speed
- `autoplay` -> automatically play the audio
- `loop` -> continuously play the audio; **Not recommended**
- you can give the fallback type also

```html
<body>
    <p>sample audio</p>
    <audio controls autoplay loop>
        <source src="music/sample_audio.mp3" type="audio/mpeg">
        <source src="music/sample_audio.wav" type="audio/wav"> <!-- backup -->
    </audio>
</body>
```