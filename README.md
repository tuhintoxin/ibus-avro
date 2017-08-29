# Avro phonetic for Linux in IBus
Avro phonetic implementation for Linux in IBus.

## Installation

1. Open terminal/package manager and install following packages:
 
		git 
		libibus-1.0-5
		libibus-1.0-dev
		ibus
		automake 
		autoconf
		gjs
		gir1.2-gjsdbus-1.0
		gir1.2-ibus-1.0

    __For Ubuntu 12.04__
    
    	sudo apt-get install git ibus libibus-1.0-dev automake autoconf gjs gir1.2-gjsdbus-1.0 gir1.2-ibus-1.0
	
   
   __For Arch Based Linux (Manjaro, AntergOS)__
    
    	sudo pacman -S git ibus automake autoconf gjs
	
   
   __For other linux distributions__
    
    You'll need all related build tools like `automake`, `autoconf` etc...
    and Latest __IBus__ from _git_ compiled with _gobject-introspection_ support enabled.



2. Now give the following commands step-by-step:

   
   __For Debian & Ubuntu Based Distros___

		git clone git://github.com/tuhintoxin/ibus-avro.git
		cd ibus-avro
		aclocal && autoconf && automake --add-missing
		./configure --prefix=/usr
		sudo make install
		sudo rm -rf ibus-avro/ (or delete ibus-avro folder from home folder)
		
   
    __For Arch Based Distros___

		git clone git://github.com/tuhintoxin/ibus-avro.git
		cd ibus-avro
		makepkg -si
		sudo rm -Rf ibus-avro/ (or delete ibus-avro folder from home folder)


## Usage Debian & Ubuntu Based Distros
 1. Run __IBus__ (`Applications -> System Tools -> IBus`) from _Dash_
 2. Open __IBus__ `Preferences` from the top panel icon  
 3. Go to `Input method`
 4. `Select an input method -> Bengali -> Avro`
 5. Now Click `Add` button to add __Avro__ to the list
 6. Now restart __IBus__ from the top panel icon (`Right Click -> Restart`)
 7. Now Press `Ctrl+Space` to toggle between _English_ and _Avro_ (Bengali)
 8. Enjoy __Avro Phonetic!__


 ## Usage Arch based distros
 1. Run __IBus__ (`Search for ibus preferances and open it `)
 2. Go to `Input method`
 3. `Select an input method -> Bengali -> Avro`
 4. Now Click `Add` button to add __Avro__ to the list
 5. Now restart __IBus__ open terminal and write command (`ibus restart`)
 6. Now Press `Ctrl+Space` to toggle between _English_ and _Avro_ (Bengali)
 7. Enjoy __Avro Phonetic!__

## Contributors
 
__IBus Engine__ by __Sarim Khan__ <sarim2005@gmail.com>

[__Avro JavaScript Phonetic Library__](https://github.com/torifat/jsAvroPhonetic) by [__Rifat Nabi__](https://github.com/torifat)

__Avro Phonetic Dictionary Search Library__ by [__Mehdi Hasan Khan__](https://github.com/omicronlab)


_Licensed under Mozilla Public License 1.1 ("MPL"), an open source/free software license._
