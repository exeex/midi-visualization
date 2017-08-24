# midi-visualization
A python package for midi-visualization which works with numpy, matplotlib and mido

You must install *numpy*, *matplotlib* and *mido* before you use it.

If you have a script which parse midi files with mido.
You can just use this:
```
from roll import MidiFile
```
to replace mido.MidiFile



# How to use it?
Just see the __main__ block in the script
You can just run the script to see how it works

if __name__ == "__main__":
    mid = MidiFile("test_file/1.mid")

    # get the list of all events
    # events = mid.get_events()

    # get the np array of piano roll image
    roll = mid.get_roll()

    # draw piano roll by pyplot
    mid.draw_roll()
