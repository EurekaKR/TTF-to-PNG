TTF-to-PNG for Korean
=====================

A PNG letter generator for icon fonts.

## What

You can extract `.png` files of korean letters from a `.ttf` font file. It is useful to obtain icon images from an icon font.

## Installation

### ImageMagick

There are a lot of ways for installation. 

- Homebrew

		brew install imagemagick

- Cactuslab's installer

	- [ImageMagick installer for Mac OS X](http://cactuslab.com/imagemagick/)

- Debian based Linux  
```
	apt-get install imagemagick
```
- RHEL based Linux  
```
	yum install ImageMagick
```
### FontTools

	pip install fonttools

### TTF-to-PNG for Korean

    git clone https://github.com/JimJeon/TTF-to-PNG.git

## Usage

1. Install `.ttf` font by fontbook.

2. Execute following command.

	    ./ttf2png.py [INSTALLED_FONT_PATH] [FONT_SIZE] 

	- You can find `INSTALLED_FONT_PATH` by the executing following command.

			convert -list font

		Output:
		
			Font: Verdana
			  family: Verdana
			  style: Normal
			  stretch: Normal
			  weight: 400
			  glyphs: /Library/Fonts/Verdana.ttf <-INSTALLED_FONT_PATH

3. Check under the `./images` dir.

## Environment

- OSX : 10.10 (Any OS that can use imagemagick)
- Python : 3.6.2
	- It may work on other version's OSX or Python.

## License

- MIT

