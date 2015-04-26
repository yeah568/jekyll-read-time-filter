# jekyll-read-time-filter
A Jekyll/Liquid filter to calculate the read time of an article based on the formula [used by Medium](https://medium.com/the-story/read-time-and-you-bc2048ab620c).

TL;DR: 275 WPM, add 12 seconds for first image, 11 for next, etc., down to a minimum of 3 seconds per image

## Installation
Just drop read_time.rb into your _plugins folder. Simple as that!

## Usage
```
{{ page.content | read_time }}
```
Note: this plugin requires img tags to be in the form of `<img ... />`. If you're using this on a post listing page, make sure to markdownify the post content first.
