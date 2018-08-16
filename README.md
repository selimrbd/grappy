# grappy

small CLI program written in python for downloading media content from internet and applying basic transformations to it.
This is basically a wrapper around core functionalities of [moviepy](https://github.com/Zulko/moviepy) and [pytube](https://github.com/nficano/pytube), use those packages directly if you are looking for the core functionalities.

## Usage

### To download a video from youtube

```grappy dl https://www.youtube.com/watch?v=dAxZBkmojbw --t1 1:46 --t2 1:53 --name "hoan_move_1" ```

* --t1 and --t2 (optional): specify the portion of the video you want to keep
* --name (optional): if not specified, the same as the youtube video

### To cut an existing video

```grappy cut path/to/myvid --t1 1:12 --t2 1:49```

### configuration

See *config.py* to specify a default folder where to move downloaded videos

## Milestones

### First milestone

* :heavy_check_mark: Download a full youtube video
* :heavy_check_mark: Crop a video between 2 given timestamps
* :heavy_check_mark: Download a youtube video and directly specify the cropping in the arguments

### Second milestone

* :white_check_mark: convert a video to audio directly
* :white_check_mark: download a full playlist of videos to audio format

### Further improvements

* DL videos from facebook, instagram, soundcloud, ...
* synchronize downloaded music with spotify

##  Resources

* [DL public youtube videos](https://pythontips.com/2018/04/23/reverse-engineering-facebook-video/)
* [cut ou portion of video](https://stackoverflow.com/questions/37317140/cutting-out-a-portion-of-video-python)
* [pytube: DL youtube videos](https://github.com/nficano/pytube)
