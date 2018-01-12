# Jump Impulse Lab
The files and diagrams for the jump impulse lab at the University of Tulsa

The main document is JumpingImpulse.lyx

## Tools to Build the Handout

The following tool is needed to compile the LyX file into a pdf on Windows 10

  - LyX 2.2.3 ftp://ftp.lyx.org/pub/lyx/bin/2.2.3/LyX-223-Bundle-2.exe

This will install MikTeX, which is the windows package for LaTeX. MikTeX can be set up to install all missing packages on the fly, but the following steps install the needed packages (plus a little more).

Steps:
1. Open the MikTeX Package Manager (ADMIN)
2. Enter `koma` in the name filter box and install all the resulting packages. This installs the nice looking base class of Koma-Script.
3. Enter `pst` in the name filter box and install all the resulting packages. This installs all the drawing packages for PSTricks, which may take a while. The pst-geo package is large and not needed. 
4. Enter `url` in the name filter and install all the resulting packages.
5. Enter `xcolor` in the name filter and install all the resulting packages.
6. Enter `multido` in the name filter and install the resulting packages.
7. Close the MikTeX Package Manager
8. Open LyX
9. Select `Reconfigure` from the Tools menu. This updates LyX with the new classes of documents installed. 
10. Restart LyX
11. Open LyX and the JumpingImpulse.lyx file
12. Select `File` -> `Export` -> `PDF (ps2pdf)` to typeset the document. Other PDF exporters won't work because of the PSTricks in the document.
