---
tags:
    - media
---
# Planning for Audio and Video Hosting

Mukurtu CMS provides two options for managing audio and video files: direct upload, or external hosting with a third party service.

While most media assets can be uploaded directly, even access copies of videos will have very large file sizes. In many cases it is more cost-effective to use an external video hosting provider than paying for additional in-site storage.

You also want to ensure that your users have a good playback or streaming experience, regardless of their internet bandwidth, speed, or service.. While small uploaded video files may play fine, externally hosted videos usually load faster and play more reliably since those services are optimized for video streaming.

Some audio files are large enough that external hosting might also be worth considering.

## Direct upload

- Video files uploaded directly to your Mukurtu CMS site are stored and managed the same as any other media assets.
- Ensure that your hosting plan provides sufficient space for large video files.
- The default maximum upload size for a single file is 128MB, but your system/server administrator should be able to configure support for larger individual uploads. For more information on site configuration, visit **ARTICLE FOR THIS**
- Directly uploaded videos will use the default HTML5 video player.

## External hosting

- Mukurtu CMS supports external hosting through Vimeo and Youtube for videos and SoundCloud for audio files.
- To use one of these providers, you need to create an account with the respective service. These services over a range of free and paid accounts, each with their own features and limitations.
- SoundCloud, Vimeo, and YouTube support some type of  “private” hosting, so your videos will not be shown on their own platforms, but can still be accessed through your Mukurtu CMS site.

    !!! tip
        For more information on privacy settings for externally hosted media, visit [SoundCloud Privacy Settings](SoundCloudPrivacySettings.md), [Vimeo Privacy Settings](VimeoPrivacySettings.md), or [YouTube Privacy Settings](YoutubePrivacySettings.md).

- Externally hosted audio files and videos do not use storage space on your Mukurtu CMS site, but if they are removed from the hosting platform they will no longer be available through your Mukurtu CMS site.
- Externally hosted audio files and videos will use the native, embedded player provided by each platform.