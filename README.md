# gl

```
tuning E3A3D4G4B4E5
capo 1
key G
tempo 120bpm

G

Em

D

A

Asus4

000220
001220

...



$chord Am = 012200
$note ReDiezFive = D#5
$note MyNote = E5

key [optional data] {
	[block body]
}
```

```
#include <predefined-chords.gl>
track {
	tempo 120bpm
	bar-size 4/4

	define {
		$Am:chord = 012200
		$ReDiezFive:note = D#5
		$MyNote:note = E5
	}

	instrument Guitar Hetfield {
		tuning E3A3D4G4B4E5
		capo 1
		key G
		
		bars [
			bar {
				chord $Am {
					len 4
				}
				chord 032200 {
					len 4
					dot true
				}
			}
			bar {
				chord $Am {
					len 4
				}
				chord 032200 {
					len 4
					dot true
				}
			}
			bar {
				chord $Am {
					len 4
				}
				chord 032200 {
					len 4
					dot true
				}
			}
			bar {
				chord $Am {
					len 4
				}
				chord 032200 {
					len 4
					dot true
				}
			}
		]
	}

	instrument Guitar Hetfield {
		tuning Standard
		capo 1
		key G
		tempo 120bpm
		BarSize 4/4
		
		define {
			$Em:chord = 000220
			$ReDiezFive:note = D#5
			$MyNote:note = E5
		}
	}
}

```
