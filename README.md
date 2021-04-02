Web browsers suck
The modern web is slow and bloated. It is coated in malicious trackers and adverts. The traditional method of browsing (using graphical web browsers) is also clunky. Moreover, algorithms, clickbait and biased/unfactual news are used to further manipulate us. There are a few ways to go about solving this issue:
1. Use an alternative web protocol such as [Gopher](https://www.youtube.com/watch?v=-mzjYC5aWkk) or [Gemini](https://www.youtube.com/watch?v=K-en4nEV5Xc) - *although seemingly promising, these will likely never become mainstream*
2. Use a text-based browser such as Lynx or w3m - *plenty of websites do not function well without JavaScript*
3. Use superior software where possible (see below) - *can be tinkered with and designed for their specific purpose*

Also, I'd like to apologise for the overuse of the word *'bloat'*. It is used a lot but only for the lack of a better word.

# Superior software
Most of these tools are commandline-based because I prefer using the terminal but I have included a few graphical applications as well. Also, all of these applications are pretty easy to configure; none of them require you to deal with some complex API (not even the YouTube clients, except for youtube-viewer).

* Basic searches: [Tuxi](https://github.com/Bugswriter/tuxi)
* Images: [e.xec.sh](https://github.com/mattLLVW/e.xec.sh) (if you input the curl command with `?img=true` at the end) or [gallery-dl](https://github.com/mikf/gallery-dl) *or* [gimage](https://github.com/koalagang/gimage) (my own project - a work-in-progress)
* Weather forecast: [wttr.in](https://github.com/chubin/wttr.in)
* Cryptocurrency rates: [rate.sx](https://github.com/chubin/rate.sx) *or* [Coinmon](https://github.com/bichenkk/coinmon) *or* [Cointop](https://github.com/miguelmota/cointop)
* YouTube: [youtube-dl](https://github.com/ytdl-org/youtube-dl) *or* [youtube-viewer](https://github.com/trizen/youtube-viewer) *or* [pipe-viewer](https://github.com/trizen/pipe-viewer) *or* [FreeTube](https://github.com/FreeTubeApp/FreeTube)  *or* [NewPipe](https://github.com/TeamNewPipe/NewPipe) (an Android app) *or* [yt](https://github.com/sayan01/scripts/blob/master/yt) *or* [Ytfzf](https://github.com/pystardust/ytfzf) (has thumbnail support using Ueberzug) *or* [Streamlink](https://github.com/streamlink/streamlink) (see below NOTE section) - *TIP*: when using pipe-viewer, you can use [Invidious](https://github.com/iv-org/invidious) instead of YouTube by parsing the `--invidious` flag. You can also use FreeTube with Invidious. *Another TIP*: when using Ytfzf, if you want to use the J and K keys (vim keys) instead of the up and down keys, simply hold down ctrl while using J and K
* Emailing: [NeoMutt](https://github.com/neomutt/neomutt) *or* [Thunderbird](https://www.thunderbird.net/en-GB/) *or* [Mailspring](https://github.com/Foundry376/Mailspring) - *TIP*: use [mutt-wizard](https://github.com/LukeSmithxyz/mutt-wizard) to easily configure NeoMutt
* COVID-19 stats: [Coronavirus Tracker CLI](https://github.com/sagarkarira/coronavirus-tracker-cli)
* Calendar: [Calcurse](https://github.com/lfos/calcurse) (TUI) *or* [Gnome Calendar](https://wiki.gnome.org/Apps/Calendar) (Gtk)
* Google Translate: [Translate Shell](https://github.com/soimort/translate-shell) *or* [Tuxi](https://github.com/Bugswriter/tuxi) - *TIP*: you can also use Translate Shell as a dictionary if you add the '-d' flag, e.g. `trans -d stupendous`
* Finding emojis: [emoj](https://github.com/sindresorhus/emoj) *or* [DmenuUnicode](https://github.com/LukeSmithxyz/voidrice/blob/master/.local/bin/dmenuunicode) - *TIP*: emoj uses nodejs but DmenuUnicode is just a simple (18 lines, 9 if you exclude comments and empty lines) shell script so it would probably be preferred
* Memes: [parrot.live](https://github.com/hugomd/parrot.live) *or* [e.xec.sh](https://github.com/mattLLVW/e.xec.sh) *or* [dankcli](https://github.com/sggts04/dankcli) *or* [Ricksay]() *or* Reddit *(see below)*
* Reddit: [redyt](https://github.com/Bugswriter/redyt) *or* [Reddsaver](https://github.com/manojkarthick/reddsaver) *or* [TUIR](https://gitlab.com/ajak/tuir) *or* [Slide](https://github.com/ccrama/Slide) (an Android app)
* Twitter: [Rainbow Stream](https://github.com/orakaro/rainbowstream)
* Facebook: [Facebook CLI](https://github.com/specious/facebook-cli)
* Instagram: [InstaLooter](https://github.com/althonos/InstaLooter)
* Finding people on social media: [Sherlock](https://github.com/sherlock-project/sherlock)
* Twitch: [Twire](https://f-droid.org/en/packages/com.perflyst.twire/) (an Android app) *or* [Streamlink](https://github.com/streamlink/streamlink) (see below NOTE section)
* Git: [GitHub Cli](https://github.com/cli/cli) *or* [Tig](https://github.com/jonas/tig) *or* [GitHub-Tui](https://github.com/skanehira/github-tui) *or* [Lazygit](https://github.com/jesseduffield/lazygit) *or* [Lab](https://github.com/zaquestion/lab)
* E-books: [calibre](https://calibre-ebook.com/) *or* [FanFicFare](https://github.com/JimmXinu/FanFicFare) *or* [calbredb](https://manual.calibre-ebook.com/generated/en/calibredb.html) - *TIP*: calibre also has a [portable version](https://calibre-ebook.com/download_portable) which can be run on any Windows computer. *Another TIP*: [calibre can process RSS feeds](https://manual.calibre-ebook.com/news.html). *Another TIP*: calibredb, is not very featureful; it is useful because it is a fast CLI tool but it is recommended that you also use calibre along with it.
* [RSS](https://en.wikipedia.org/wiki/RSS): [Newsboat](https://github.com/newsboat/newsboat) (TUI) *or* [Sfeed](https://codemadness.org/sfeed-simple-feed-parser.html) (TUI) *or* [Neix](https://github.com/tomschwarz/neix) (TUI) *or* [Akregator](https://userbase.kde.org/Akregator) (Qt) *or* [Newsflash](https://gitlab.com/news-flash/news*flash*gtk) (Gtk) *or* [calibre](https://manual.calibre-ebook.com/news.html) (see above 'E-books' section) - *TIP*: RSS feeds are very useful if you like to read blogs or news but can also be used for YouTube channels so you don't have to have a YouTube account to subscribe to YouTubers. You can also add Reddit pages to your RSS feed. *Another TIP*: you can add a [readability](https://pypi.org/project/readability/) macro to newsboat to remove clutter; for more see [this](https://www.youtube.com/watch?v=qPiE1JUgsBg) video and my [newsboat config](https://github.com/koalagang/dotfiles/blob/main/newsboat/config). Note that the AUR package is called `python-readability-lxml`.
* Documenation/help: [Man pages](https://en.wikipedia.org/wiki/Man_page) *or* run '--help' at the end of a command *or* [cheat.sh](https://github.com/chubin/cheat.sh)  *or* [tldr](https://github.com/tldr-pages/tldr) *or* [cheat](https://github.com/cheat/cheat) *or* Stackoverflow (see below) - *TIP*: you can [use a different manpager](https://www.youtube.com/watch?v=ab3rY0X5kD4) if you don't like less
* Stackoverflow: [so](https://github.com/samtay/so) *or* [rebound](https://github.com/shobrook/rebound)
* Podcasts: [Castero](https://github.com/xgi/castero)
* Office: [LibreOffice](https://www.libreoffice.org/) *or* [sc-im](https://github.com/andmarti1424/sc-im) (for spreadsheets) *or* [LaTeX](https://www.latex-project.org/) *or* [Groff](https://www.gnu.org/software/groff/) *or* [sent](https://tools.suckless.org/sent/) (for presentations)
* QR code generator: [QRenco.de](https://github.com/chubin/qrenco.de) - *TIP*: it doesn't say it explicitly on the GitHub page (it's shown in small text on an image) but you can run `curl qrenco.de/insert-your-data-here` to generate a QR code without downloading the application
* Pastebin: [TermBin](https://www.termbin.com/)
* Password Managers: [KeePassXC](https://github.com/keepassxreboot/keepassxc) (Gtk) *or* [pass](https://www.passwordstore.org/) (CLI)
* Manga/Webtoons: [gallery-dl](https://github.com/mikf/gallery-dl) *or* [Manga-Downloader](https://github.com/jiaweihli/manga_downloader) - *TIP*: as of when I am writing this, Manga-Downloader is undergoing a rewrite and the AUR package is not only out-of-date but fails to build. For this reason, I recommend gallery-dl and then maybe come back to Manga-Downloader later.
* Dictionary: [Translate Shell](https://github.com/soimort/translate-shell) (if you use the `-d` flag) *or* [dictd](https://github.com/mkuhn/dict) (aka 'dict') - *TIP*: as the usage of dictd is not entirely intuitive, you may wish to consult the [Arch Wiki](https://wiki.archlinux.org/index.php/Dictd) or [this](https://www.youtube.com/watch?v=DvACLz06W2o) video for documentation. *Another TIP*: ***dict can be used with curl*** instead of downloading it if you input `curl dict://dict.org/d:<your-query>`
* URL shortener: [Null Pointer](http://0x0.st/)
* News: use an RSS feed (see above) *or* [getnews.tech](https://github.com/omgimanerd/getnews.tech)
* Business card: [Bryan Jenks' business card](https://github.com/tallguyjenks/BusinessCard) (this is obviously just Bryan Jenks' business card but you could easily fork it to make your own)

**NOTE**: [Streamlink](https://github.com/streamlink/streamlink) is a CLI tool which supports *many* different streaming services (too many to list on this page) - the full list can be found [here](https://streamlink.github.io/plugin_matrix.html). For a simple script to make using it simpler, see [fzstream](https://github.com/koalagang/fzstream).

# Installation
***Everyone*** should be using a package manager. For the Linux and BSD people, what package manager you should be using obviously depends on your distro. Experienced macOS users will know of [Homebrew](https://brew.sh/) (which is also available for Linux, btw). Windows users should consider using [Scoop](https://scoop.sh/) *or* [Chocolatey](https://chocolatey.org/). Microsoft also has its own official package manager called [winget](https://github.com/microsoft/winget-cli), but it is in early development and lacks many basic features. [Here](https://www.youtube.com/watch?v=DVeNUAFgHQc) is a good video covering it at its current state.

Many of the software in the list of 'superior software' usually instruct you to use a language specific package manager, such as npm or pip3. Fortunately for Arch/Arch-based users, plenty of these software are also available on the AUR; I recommend you download it from there if this is the case. People who are not using Arch will, however, probably have to download the specific package manager or compile from source.

# If you must use a web browser
Use one or more of the following browsers:
* [Brave](https://brave.com/) (a secure, fast & private Chromium-based web browser)
* [LibreWolf](https://librewolf-community.gitlab.io/) (a fork of Firefox, focused on privacy, security and freedom)
* [Qutebrowser](https://qutebrowser.org/) (a lightweight keyboard-driven browser with a minimal GUI)
* [Tor Browser](https://www.torproject.org/) (the most private browser in the world; powerful for countering government censorship and surveillance)
* [Bromite](https://www.bromite.org/) (a Chromium-based Android browser with ad blocking and enhanced privacy)
* [Lynx](https://lynx.browser.org/) (the oldest actively maintained text-based browser)
* [w3m](http://w3m.sourceforge.net/) (a text-based browser which supports image viewing)
* [Amfora](https://github.com/makeworld-the-better-one/amfora) (a fancy terminal browser for the Gemini protocol)
* [Castor](https://git.sr.ht/~julienxx/castor) (a graphical client for plain-text protocols written in Rust with GTK. It currently supports the Gemini, Gopher and Finger protocols.)

If you are using a PC/laptop Chromium or Firefox-based browser, use one or more of following extensions:
* [uBlock Origin](https://github.com/gorhill/uBlock#ublock-origin) *or* Privacy Badger (not needed if you are on Brave)
* [Cookies AutoDelete](https://github.com/Cookie-AutoDelete/Cookie-AutoDelete)
* [Decentraleyes](https://decentraleyes.org/)
* [HTTPS Everywhere](https://www.eff.org/https-everywhere) (NOTE: Firefox and Brave have this as a built-in feature)
* [NoScript](https://noscript.net/) *or* [uMatrix](https://github.com/gorhill/uMatrix) - *TIP*: NoScript's website is hard to navigate; click [here](https://addons.mozilla.org/en-US/firefox/addon/noscript/) for the Firefox version and [here](https://chrome.google.com/webstore/detail/noscript/doojmbjmlfjjnbmnoijecmcbfeoakpjm) for the Chromium version.
* [ClearURLS] (NOTE: Firefox has this as a built-in feature)
* [Minimal](https://gitlab.com/aupya/minimal)
* [Terms of Service; Didn't Read](https://tosdr.org/) (aka ToS;DR)

Some of these browser extensions block trackers but [blocking trackers using your local host file](https://www.youtube.com/watch?v=VPfpCVW7ZvM) or even [network level blocking](https://pi-hole.net/) is better than browser-level blocking because it allows you to block tracking even on unorthodox platforms such as mobile apps or smart TVs. It also means that your adblocking is browser-agnostic; you are not forced to use Chromium or Firefox for any level of privacy. It also ensures that you don't have to cram your already bloated browser with more bloat. If you wish to use a hardened Firefox - check out [ghacks user.js](https://github.com/arkenfox/user.js) (remember to read the readme carefully; use it as a template and do not apply it to Tor Browser). Also, if you choose to go the browser extensions route: try not to plaster on too many extensions because it will only make your fingerprint more unique.

If you want up-to-date advice about online privacy - see [PrivacyTools](https://privacytools.io/).
To see how unique your browsing fingerprint is and how well you block trackers - see EFF's [CoverYourTracks](https://coveryourtracks.eff.org/).
For help with making Qutebrowser more private - see [my config.py](https://github.com/koalagang/dotfiles/blob/main/qutebrowser/config.py).

I would also suggest that you use [Surfraw](https://gitlab.com/surfraw/Surfraw/) and then alias your preferred search engine (e.g. alias ddg='sr duckduckgo' or alias wp='sr wikipedia') to make using text-based browsers more convienient.

# Is the modern web inherently bad?

Yes and no. Compared to how hard it was to gain access to information a few decades ago, the web has helped us to make many advances in developing society. It also distributes help and communication for huge amounts of people. Furthermore, it is the easiest way to find entertainment for free (in terms of money cost that is). The problem is that in the current circumstance, just by opening your web browser and loading up a page like YouTube, you are being violated. Not only are cookies which follow you around planted into your browser but YouTube uses dirty tactics to keep you on the website and continuing to earn them money; this would include the use of warm colours, big buttons, infinite scrolling pages, targeted videos, etc. Fortunately, there are people generous enough to give up their time to develope software such as those in the list. It is, however, also possible to make a well designed website.

**But how do you make a** ***good*** **website?** Here are two great examples on how a website should be designed - [Based Cooking](https://based.cooking/) and [wolfgang's blog](https://notthebe.ee/). [Here](https://www.youtube.com/watch?v=ykNEkiYr0QM) and [here](https://www.youtube.com/watch?v=N_ttw2Dihn8) are videos covering them respectively. I am of the opinion that a good website should function well in a text-based browser and these two work very nicely (at least in Lynx). That is not to say that videos and pictures are wrong to include (in fact these websites do include videos and pictures) but the point is that there shouldn't be a signficiant inconvenience in not using a graphical browser - this would mean that it should be functioning without JavaScript.

# Community-based?
Currently I am the only one working on this list but feel free to make a pull request if you think there is something else which belongs on the list.
