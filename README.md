# CompressVideo
A High-performance video compressor for Android using Hardware decoding and encoding API(MediaCodec).

# Motivation
I tried many Video compressor as expected some are not working and outdated ,some are working but not maintaing video resolutions

## Demo
![Demo](/pic/Demo.gif)

## Usage
### Call compressVideoLow, compressVideoMedium and compressVideoHigh that indicates 3 quality of compressing.
        VideoCompress.compressVideoLow(String srcPath, String destPath, new VideoCompress.CompressListener() {
            @Override
            public void onStart() {
                //Start Compress
            }

            @Override
            public void onSuccess(String compressVideoPath) {
                //Finish successfully
            }

            @Override
            public void onFail() {
                //Failed
            }

            @Override
            public void onProgress(float percent) {
                //Progress
            }
        });

## Performance

I compress a video which is 2.62MB(00:0:12).

And it took 8 seconds for compressing.

The result of compressing is 479KB.

So it's a great job by MediaCodec :) .

## License
```
Copyright 2017 Vincent Woo

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
