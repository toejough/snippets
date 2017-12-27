# snippets
helpful snippets that I keep forgetting

these are things that I use often enough that I want quick access to them, but not often enough (at least at time of recording) that I remember them on my own.

The idea is that if I need somethign I know I already looked up, I'll add it here.  Hopefully that'll mean that I can get it more quickly in the future, and that will lead to me using the useful thing more often, and that'll lead to me actually remembering it, and I'll only ever be referring regularly to things at the bottom of the list (which'll make it even easier to find).

That's the goal.

Feel free to suggest other helpful snippets, but this is by design and intent really opinionated.  If I get a suggestion for something I actually decide I should use, I try it, and it's great, I'll add it iff I need to use it again and can't remember it.

# The actual snippets

* python3 SimpleHTTPServer: `python3 -m http.server`
* rename your current local branch in git: `git branch -m <new-name>`
* take notes on a commit in git `git notes add|append -m "<note>"`
* view last notes in git `git notes show` or all notes with commits `git log`
* add an upstream github origin: `git remote add origin https://github.com/<person|org>/<project>.git`
* generate and push ssh key: `ssh-keygen && ssh-copy-id <remote-host>`
* get your bash script's dir, in the script: `DIR="$( cd "$( dirname "${BASH_SOURCE[0]}"  )" && pwd  )"` ([source](http://stackoverflow.com/a/246128/5372442))
* remove something from git, but not from your working tree (file system): `git rm --cached <thing>`
* expand the command line - * autocompletion - `esc *` (if you're in vim mode)
* delete lines which match a pattern in vIM: `:%g/pattern/d`
* find the active activity name in android: `adb shell dumpsys activity activities`
* get the top 10 time-sucks in a python function: `cProfile.run("<call>", "stats"); pstats.Stats("stats").sort_stats('tottime').print_stats(10)`
* input text in an android device via adb: `adb shell input text <text>`
* check/exit an ssh control master: `ssh -O check|exit <host>`
* show hidden files on a mac: `defaults write com.apple.finder AppleShowAllFiles YES` then right-click & relaunch finder
* run a vim command from the commandline: `vim +<command> +qall` (where `<command>` is the command you'd type at a `:` prompt within vim)
* stop OSX Photos app from launching every time you put an SD card in: `defaults -currentHost write com.apple.ImageCapture disableHotPlug -bool true`
* reset osx camera when it fails to connect: `sudo killall VDCAssistant && sudo killall AppleCameraAssistant`
