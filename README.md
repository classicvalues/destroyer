<img src='https://www.dropbox.com/s/alcqju8k9lkr3b9/destroyer-logo.png?raw=1' width='250px'/>

# Destroyer

### Open-Source Lossless Audio Player

![destroyer](https://www.dropbox.com/s/1yhcbcw2if0cwhp/destroyer.jpg?raw=1)

### v2.0 Breaking Changes:

* Swap to native HTML5 audio players (FLAC, MP4, MP3, OGG, WAV supported!)
* Seeking (finally!)
* TouchBar support for Macbook Pro!
* An actual DMG install file for Mac (wow!)
* Removal of FFPLAY and FFMEG (this should make it easier to build for all OS!)
* Removal of metadata editor (may come back!)
* Minor style tweeks

[Download for Mac](https://github.com/mashaal/destroyer/releases)

[Watch demo video on YouTube](https://www.youtube.com/watch?v=mJwW7uwNY4s)

## Getting Started:

![start](https://www.dropbox.com/s/ddtbw9jt640zand/start.gif?raw=1)

* Download and open **Destroyer**.
* Drop your music collection onto **Destroyer**.
* **Destroyer** will recursively scan your collection and build library based on metadata.

**Note:** **Destroyer** is dependant on metadata — it can process [Vorbis](https://wiki.xiph.org/Metadata) comments as well as [ID3](https://en.wikipedia.org/wiki/ID3) (1.1, 2.2, 2.3, 2.4) tags. Please ensure your collection is properly formatted.

## On Artwork:

* **Destroyer** works best when all the tracks for an album are in one flat directory.
* **Destroyer** will look for a file named `cover.jpg` in the album's directory, if `cover.jpg` not found, it will fallback to any `jpg` or `png` in directory.

## On Search:

![search](https://www.dropbox.com/s/qh218t53t38ahvq/search.gif?raw=1)

* Type anywhere in the library view to filter your collection.
* `esc` will clear your filter.

### Deving and Building

| Command            | Purpose                              |
| :----------------- | :----------------------------------- |
| `yarn build`       | Compile JS `/bundle`.                |
| `yarn build:watch` | Build project and watch for changes. |
| `yarn start`       | Start Destroyer.                     |
| `yarn pack:osx`    | Build for Mac.                       |
| `yarn pack:win`    | Build for Windows.                   |
