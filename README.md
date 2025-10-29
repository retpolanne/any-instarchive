# Instarchive

A tool for archiving Instagram posts based on Anyproto.

## About this

Instagram is a widely used social media website. A lot of people use Instagram, and it has become
a quite popular means of being up to date with your friends, family and content creators. 

Making content on Instagram is, for some people, a full-time job. 

You may think that Instagram is just brainrot, but there's actually good content there. 
Some people put a lot of effort on making actual research before making posts on Instagram, 
and a lot of these posts deserve better archival.

The big problem regarding Instagram is that it's a walled garden where information is scattered and
not properly catalogued. Information on Instagram is easily lost due to not having any easily indexable content
and relying too much on audiovisual content. 

Aside from that, Meta has been pretty harmful for initiatives such as the Internet Archive. 

You may ask why we need so much effort cataloguing content from Instagram? Well, this is our new Alexandria
library – as I've mentioned, lots of meaningful content are being created on Instagram every second and leaving
this platform is not as easy for most of these people. There's a lot of arts, music, communities bubbling on
Instagram that need to be archived – and especially outside of Instagram. 

Let's not forget that Instagram belongs to Meta, an US based company that may at any minute restrict information 
based on arbitrary rules defined by them or by the US government. 

## How we want to achieve archival

The idea is to make it as low code as possible and use Anytype as the backend powering everything.
Anytype can power the distributed information storage that we need as a backend and as a catalogue. 

The main application, Instarchive, should work as easily as:

1. You pass an Instagram URL to it;

2. Some information is gathered about the post, such as the images URLs, videos, text and other metadata;

3. Images are then processed through OCR. Videos can be transcribed. We can also make image descriptions of the content.

4. All of this content is then stored on your Anytype vault using the Anytype API. 


Regarding step 3, OCR doesn't require AI. Transcription is better done with Whisper (unfortunately),
same for image descriptions. We'll probably leave it for later and focus on OCR. 

## Challenges

- [Meta has deprecated the Basic Display API](https://developers.facebook.com/blog/post/2024/09/04/update-on-instagram-basic-display-api/) 
for Instagram, which means consumer apps will no longer work for users 
without a Business or Professional account. This is a bummer.

- Doing scraping is a bit intensive and trying to analyse the HTML is very burdensome and difficult. 

- I also don't want my account to be banned due to ToS infringement. 
