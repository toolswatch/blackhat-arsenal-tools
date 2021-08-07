# FileInsight-plugins

### Description
FileInsight-plugins is a large set of plugins for McAfee FileInsight hex editor. It adds many capabilities such as decode, decryption, decompression, searching XOR-ed text strings, scanning with a YARA rule, code emulation, disassembly, and more! It is useful for various kinds of decoding tasks in malware analysis (such as extracting malware executable files from malicious document files, deobfuscation of malicious scripts).

Currently, FileInsight-plugins has 116 plugins. The plugins provide the following functions and many other functions.

- Calculation of hash values (CRC32, MD5, SHA1, SHA256, ssdeep, imphash, impfuzzy)
- Search for XORed, bit-rotated text strings and byte arrays
- XOR while incrementing / decrementing XOR key (rolling XOR)
- Encode and decode of BASE16, BASE32, BASE58, BASE64, BASE85 with custom tables
- Encryption and decryption (AES, ARC2, ARC4, Blowfish, ChaCha20, DES, Salsa20, TEA, Triple DES, XTEA)
- Compression and decompression (aPLib, Bzip2, Deflate, Gzip, LZ4, LZMA, LZNT1, LZO, PPMd, QuickLZ, XZ, Zstandard)
- Detection of embedded files in a file
- Extraction of text strings of ASCII and UTF-16 with auto decode of hex string and BASE64 strings
- Scanning with YARA and highlighting regions that match YARA rules
- Showing file metadata
- Parsing file structure (Gzip, RAR, ZIP, ELF, PE, MBR partition table, BMP, GIF, JPEG, PNG, Windows shortcut)
- Code emulation of shellcodes and executable files (Windows (x64, x86) and Linux (x64, x86, ARM, ARM64, MIPS)) with API call tracing and capturing memory dumps
- Disassembly (x64, x86, ARM, ARM64, MIPS, PowerPC, PowerPC64, SPARC)
- Opening data with other tools such as CyberChef, IDA, and VSCode (customizable with JSON config file).
- Visualization (Bitmap, Byte histogram, Entropy graph)

FileInsight-plugins is a tool that I develop privately, not professionally developed by the organization I belong to.

### Categories
Reverse Engineering

### Black Hat sessions
[![Black Hat Arsenal](https://raw.githubusercontent.com/toolswatch/badges/master/arsenal/usa/2021.svg)](https://www.blackhat.com/us-21/arsenal/schedule/#fileinsight-plugins-decoding-toolbox-of-mcafee-fileinsight-hex-editor-for-malware-analysis-23386)

### Code
https://github.com/nmantani/FileInsight-plugins/

### Lead Developer
Nobutaka Mantani - https://github.com/nmantani

### Social Media
* [Twitter](https://twitter.com/nmantani)
