##### To show multi-subtitles for better studying experience, modify `zh-CN` or `en` to your preferred languages, then type below code to browser console. 
##### 将以下代码copy至浏览器控制台即可支持中英双语对照

```javascript
var myvideo = document.getElementsByTagName('video')[0];
for (var i = 0; i < myvideo.textTracks.length; i++) {
  ["en", "zh-CN"].indexOf(myvideo.textTracks[i].language) > -1 ? myvideo.textTracks[i].mode = "showing" : myvideo.textTracks[i].mode = "hidden";
}
```
