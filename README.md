# ffmpeg
Mirror of some FFmpeg includes and libs.
- FFmpeg is licensed under the GNU General Public License.
- FFmpeg source code is available at https://ffmpeg.org

This repository exists solely as a submodule for [this project](https://github.com/watsonbw/MBR-DAQ-App).

Retrieving your own libraries:
- The static libraries on windows are provided by `pacman`.
- The static libraries on macOS are compiled manually from source with the configuration:
```shell
./configure \
    --prefix="$(pwd)/../ffmpeg_static_output" \
    --enable-static \
    --disable-shared \
    --disable-programs \
    --disable-doc \
    --enable-gpl \
    --enable-version3 \
    --enable-videotoolbox \
    --enable-audiotoolbox
```
