
# Emulate "Use Toggle Keys" on MacOS
Emulate Windows' "Use Toggle Keys" -play beep sound when caps lock/num lock is pressed- for Karabiner-Elements.
Useful for users who want to be warned when caps/num lock key is pressed. I haven't implemented it for scroll lock key because I don't have the physical key for that. You can manually override this rule by editing the json file.


## Features
You may choose one of the three flavours:
- Play beep sound when caps/num lock is pressed.
- Show notification toast when caps/num lock is pressed.
- Play beep sound and notification toast when caps/num lock is pressed.


## Dependency
1. For rule #1
- ffmpeg library for playing sound, installed in `/usr/local/bin`.
- The beep sound itself. You'll need to save it in "~/.beep.mp3".

2. For rule #2 and #3

   No dependency. I used `sound name` property from `display notification` instead of playing an external file. I've set it to `""`, if you want to change the sound, you can declare a sound name located in `System/Library/Sounds`. For example: `sound name "Frog"`.

## Installation
1. Manual installation

   Download the json file from this repository and save it in `~/.config/karabiner/assets/complex_modifications`. Then you can load this rule under "Complex modification" screen in Karabiner-Elements.
    
## Contributing

Contributions are always welcome!

You can post issues or do a pull request to contribute. As I am not a programmer, I'll always welcome every idea.


## Acknowledgements

 - [Muhammed Zakir](https://github.com/MuhammedZakir) for giving the pointers needed for this solution in this [issue](https://github.com/pqrs-org/Karabiner-Elements/issues/3100).
 - [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
 - [Awesome README](https://github.com/matiassingers/awesome-readme)
 - [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)

