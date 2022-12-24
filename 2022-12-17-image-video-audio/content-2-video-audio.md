# Video and audio content

## The `<video>` element
* The `<video>` element allows you to embed a video 

```html
<video controls>
  <source src="rabbit320.mp4" type="video/mp4" />
</video>

```

* The features of note are:
* `src`: The src (source) attribute contains a path to the video you want to embed. It works in exactly the same way.
* `controls`: You must use the controls attribute to include the browser's own control interface. The interface includes a way to start and stop the media, and to adjust the volume.

## Other `<video>` features
* `autoplay`: Makes the audio or video start playing right away, while the rest of the page is loading. You are advised not to use autoplaying video (or audio) on your sites, because users can find it really annoying.
* `loop`: Makes the video (or audio) start playing again whenever it finishes. This can also be annoying, so only use if really necessary.
* `muted`: Causes the media to play with the sound turned off by default.
* `poster`: The URL of an image which will be displayed before the video is played. It is intended to be used for a splash screen or advertising screen.
* `preload`: Used for buffering large files; it can take one of three values:
    * `"none"` does not buffer the file
    * `"auto"` buffers the media file
    * `"metadata"` buffers only the metadata for the file

```html
<video
  controls
  autoplay
  loop
  muted
  preload="auto"
  poster="poster.png">
  <source src="rabbit320.mp4" type="video/mp4" />
  <source src="rabbit320.webm" type="video/webm" />
  <p>
    Your browser doesn't support this video. Here is a
    <a href="rabbit320.mp4">link to the video</a> instead.
  </p>
</video>

```

## The `<audio>` element
* The `<audio>` element works just like the `<video>` element, with a few small differences as outlined below.
```html
<audio controls>
  <source src="viper.ogg" type="audio/ogg" />
</audio>
```

## Display video text tracks
* To get this displayed along with the HTML media playback, you need to:
    * Save it as a `.vtt` file in a sensible place.
    * Link to the `.vtt` file with the `<track>` element. `<track>` should be placed within `<audio>` or `<video>`, but after all `<source>` elements. Use the kind attribute to specify whether the cues are subtitles, captions, or descriptions. Further, use `srclang` to tell the browser what language you have written the subtitles in. Finally, add `label` to help readers identify the language they are searching for.

* A typical WebVTT file will look something like this:
```text
WEBVTT

1
00:00:22.230 --> 00:00:24.606
This is the first subtitle.

2
00:00:30.739 --> 00:00:34.074
This is the second.

…

```
* Example: note that video and audio can specified with multiple sources to support many media format.

```html
<video controls>
  <source src="example.mp4" type="video/mp4" />
  <source src="example.webm" type="video/webm" />
  <track kind="subtitles" src="subtitles_es.vtt" srclang="es" label="Spanish" />
</video>

```