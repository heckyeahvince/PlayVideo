# Play Video

This assignment illustrates how to use play video. 

## Keypoint

```java
private void playVideo(){
        VideoView videoview = (VideoView) findViewById(R.id.video);
        videoview.setVideoURI(Uri.parse("android.resource://" + getPackageName() + "/" + R.raw.lovestory));
        videoview.setOnPreparedListener(new MediaPlayer.OnPreparedListener() {

            @Override
            public void onPrepared(MediaPlayer mp) {
                mp.start();
            }
        });
    }
```
