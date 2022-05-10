# Event Data
```js
yt-navigate-finish: {
  detail: {
    pageType: browse | watch | channel | shorts | search
    // watch covers clips, watch & playlists
  }
}
yt-navigate-start: {
  detail: {
    pageType: browse | watch | channel | shorts
  }
}
yt-navigate: {
  detail: {
    endpoint: {
      watchEndpoint: {
        videoID: string
      }
    }.
    playerResponse: {
       videoDetails: {
         videoId: string,
         title: string,
         channelId: string,
         lengthSeconds: int,
         shortDescription: string,
       }
    }
  }
}
yt-player-updated: {
  detail: playerClient
}

### function
playerClient: {
  // https://developers.google.com/youtube/iframe_api_reference#Operations
    "getAdState",
    "getVideoData",
    "getPlayerState",
    addEventListener()
}
```
# playerClient Events

- onVideoProgress
- onAdStart
- onAdEnd
- onStateChange
- onLoopRangeChange