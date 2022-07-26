# chinny555.github.io
<!DOCTYPE html>
<html>
  <head>
    <title>Spotify Web Playback SDK Quick Start</title>
  </head>
  <body>
    <h1>Spotify Web Playback SDK Quick Start</h1><script src="https://sdk.scdn.co/spotify-player.js"></script>
  </body>
</html>
window.onSpotifyWebPlaybackSDKReady = () => {
  const token = '[My access token]';
  const player = new Spotify.Player({
    name: 'Web Playback SDK Quick Start Player',
    getOAuthToken: cb => { cb(token); },
    volume: 0.5
  });
