# LZWFixedCompression
LZW compression algorithm uses 12 bit compression table

Command line arguments to run:
To compress a file:
args[2]: c
args[3]: file to compress

To decompress that same file:
args[2]: e
args[3]: file to decompress

The program opens up a file to compress, runs the LZW algorithm with a 12 bit integer size (up to 4096 table entries),
then saves the result in the current filename + ".lzw". The algorithm works to compress .txt files, but will most likely
not shrink a .docx file or .gif file.

Once the compression version is expanded, it will recreate the original file with an identical size to the original.
file.txt.lzw would decompress and be saved into 2file.txt.
