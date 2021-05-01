# Joke Teller

It tells you programming jokes using the text-to-speech API([VoiceRSS](http://www.voicerss.org/)). HTML, SCSS and Vanilla Javascript were used.

If you want to run this project, you need modify `tellMe()` function in `js/script.js`. Get VoiceRSS API key and add it to `tellMe()` function.

```js
function tellMe(joke) {
  VoiceRSS.speech({
    key: "<YOUR API KEY>", // This line needs to be modified
    src: joke,
    hl: "en-us",
    r: 0,
    c: "mp3",
    f: "44KHZ_16bit_stereo",
    ssml: false,
  });
}
```

![Desktop Preview](images/desktop-preview.PNG)
