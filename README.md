# TalosString

Azure Talos is an expressive multi-string mechatronic chordophone. This ChucK class was developed throughout its construction to control each one of its string units.

## Adding the class to your ChucK project:

1. Copy the "TalosString.ck" file to your project folder (or the intended location).

2. Add the TalosString class to your ChucK project using `Machine.add()` commands.

## Using the class:

1. Declare a TalosString instance.

`TalosString talos`

2. Initialize the string unit using the `init()` function (with the string number and the port as arguments).

`talos.init(1, 0)`

3. Disable or enable performance modes by passing a 0 (off) or a 1--127 (on) value. Currently available modes: 20 - tremolo, 21 - palm mute, 22 - ghost notes, 23 - slide speed.

`talos.setMode(20, 0)`

4. Call the `pluck()` function with position, velocity, and length as arguments to play the string.

`talos.pluck(0, 80, 2::second)`

5. Additional utility functions are available in the "TalosString.ck" class file.

## Examples:
Please refer to [Azure Talos' CAAC repository](https://github.com/jpyepez/AzureTalosCAAC) for examples using this ChucK class.
