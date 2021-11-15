# WordGrinder installation with patches. 

## Prerequisiti:

###ninja:

- linux —> `sudo apt-get install -y ninja-build`
- mac —> `brew install ninja`

###ncurses:

- linux —> `sudo apt-get install libncurses5-dev libncursesw5-dev`
- mac —> `brew install ncurses`

###zlib:

- linux —> `sudo apt install zlib`
- mac —> `brew install zlib`

###lua:
- linux —> `sudo apt install lua5.3`
- mac —> `brew install lua`

## Compilare wordgrinder con patches
	git clone https://github.com/davidgiven/wordgrinder.git
	cd wordgrinder
	micro src/lua/document.lua  (cambiare in "false" la riga 704)
	make all PREFIX=/usr && sudo make install PREFIX=/usr
