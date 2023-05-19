The [`min-content`](https://developer.mozilla.org/docs/Web/CSS/min-content) keyword will make a track as small as it can be without the track content overflowing. Changing the example grid layout to have three column tracks all at `min-content` size will mean they become as narrow as the longest word in the track.

- In the phrase 'CSS is awesome', the word awesome would be the `min-content`.

The [`max-content`](https://developer.mozilla.org/docs/Web/CSS/max-content) keyword has the opposite effect. The track will become as wide enough for all of the content to display in one long unbroken string. This might cause overflows as the string will not wrap.

- This is the maximum size the content of the box is asking for or has specified. It's a sentence at its widest or an image at its widest.

The [`fit-content()`](https://developer.mozilla.org/docs/Web/CSS/fit-content()) function acts like `max-content` at first. However, once the track reaches the size that you pass into the function, the content starts to wrap. So `fit-content(10em)` will create a track that is less than 10em, if the `max-content` size is less than 10em, but never larger than 10em.

