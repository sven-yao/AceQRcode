AceQRcode
=========

开源QR编码库libqrencode windows版本(VS2012)



//目录结构解析


3rdparty / getopt

linux命令行解析库(getopt.h)。 (windows移植版)


3rdparty / pnglib

qr编码中用到的pnglib库所需文件，及pnglib中使用的zlib库文件

 
 
 
================================================================== 
    qrencode  --help        
    -----------------------
	qrencode version 3.4.3
	Copyright (C) 2006-2012 Kentaro Fukuchi
	Usage: qrencode [OPTION]... [STRING]
	Encode input data in a QR Code and save as a PNG or EPS image.

	  -h           display this message.
	  --help       display the usage of long options.
	  -o FILENAME  write image to FILENAME. If '-' is specified, the result
				   will be output to standard output. If -S is given, structured
				   symbols are written to FILENAME-01.png, FILENAME-02.png, ...
				   (suffix is removed from FILENAME, if specified)
	  -s NUMBER    specify module size in dots (pixels). (default=3)
	  -l {LMQH}    specify error correction level from L (lowest) to H (highest).
				   (default=L)
	  -v NUMBER    specify the version of the symbol. (default=auto)
	  -m NUMBER    specify the width of the margins. (default=4 (2 for Micro))
	  -d NUMBER    specify the DPI of the generated PNG. (default=72)
	  -t {PNG,EPS,SVG,ANSI,ANSI256,ASCII,ASCIIi,UTF8,ANSIUTF8}
				   specify the type of the generated image. (default=PNG)
	  -S           make structured symbols. Version must be specified.
	  -k           assume that the input text contains kanji (shift-jis).
	  -c           encode lower-case alphabet characters in 8-bit mode. (default)
	  -i           ignore case distinctions and use only upper-case characters.
	  -8           encode entire data in 8-bit mode. -k, -c and -i will be ignored.
	  -M           encode in a Micro QR Code.
	  -f  --foreground=RRGGBB[AA]
	  -b  --background=RRGGBB[AA]
				   specify foreground/background color in hexadecimal notation.
				   6-digit (RGB) or 8-digit (RGBA) form are supported.
				   Color output support available only in PNG and SVG.
	  -V           display the version number and copyrights of the qrencode.
	  [STRING]     input data. If it is not specified, data will be taken from
				   standard input.
