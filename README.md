# just_audio_background ryanheise bug on live streaming (only for sample)

This package only sample to showing ryanheise bug on live streaming radio app..

I was change on Audio Source URL :

```dart
AudioSource.uri(
  Uri.parse('https://example.com/song1.mp3'),
  tag: MediaItem(
    // Specify a unique ID for each media item:
    id: '1',
    // Metadata to display in the notification:
    album: "Album name",
    title: "Song name",
    artUri: Uri.parse('https://example.com/albumart.jpg'),
  ),
),
```

To :

```dart
AudioSource.uri(
  Uri.parse('https://n01.radiojar.com/4ywdgup3bnzuv?rj-tok=AAABe7D30VkAfEM266RZXz6WWQ&rj-ttl=5'),
  tag: MediaItem(
    // Specify a unique ID for each media item:
    id: '1',
    // Metadata to display in the notification:
    album: "Album name",
    title: "Song name",
    artUri: Uri.parse('https://example.com/albumart.jpg'),
  ),
),

This URL is a live Radio Streaming Apps

https://n01.radiojar.com/4ywdgup3bnzuv?rj-tok=AAABe7D30VkAfEM266RZXz6WWQ&rj-ttl=5
