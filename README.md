# echo

## A Linux-style echo utility for Mike Riley's Elf/OS.

echo displays the command tail, with backslash substitution.

### SYNOPSIS

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;echo \[SHORT-OPTION\]... \[STRING\]...

### DESCRIPTION
<table>
<tr><td colspan=2>Echo the STRING(s) to standard output.</td></tr>
<tr><td>-e</td><td>enable interpretation of backslash escapes</td></tr>
<tr><td>-E</td><td>disable interpretation of backslash escapes (default)</td></tr>
<tr><td>--help</td><td>display this help and exit</td></tr>
<tr><td colspan=2>If -e is in effect, the following sequences are recognized:</td></tr>
<tr><td>&bsol;&bsol;</td><td>backslash</td></tr>
<tr><td>&bsol;a</td><td>alert (BEL)</td></tr>
<tr><td>&bsol;b</td><td>backspace</td></tr>
<tr><td>&bsol;c</td><td>produce no further output</td></tr>
<tr><td>&bsol;e</td><td>escape</td></tr>
<tr><td>&bsol;f</td><td>form feed</td></tr>
<tr><td>&bsol;n</td><td>new line</td></tr>
<tr><td>&bsol;r</td><td>carriage return</td></tr>
<tr><td>&bsol;t</td><td>horizontal tab</td></tr>
<tr><td>&bsol;v</td><td>vertical tab</td></tr>
<tr><td>&bsol;0NNN</td><td>byte with octal value NNN (1 to 3 digits)</td></tr>
<tr><td>&bsol;xHH</td><td>byte with hexadecimal value HH (1 to 2 digits)</td></tr>
</table>
<br>
The source was assembled with a modified version of the A18 assembler.
The header files `bios.inc` and `kernel.inc` are slightly modified
versions of Mike Riley's files; the `#ifdef...#endif` bits have been
removed or unconditionally included as appropriate, `#define`s changed
to `equ`, and upper/lower casing was made consistent.
