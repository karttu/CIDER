
How to proceed?

First, get scsh (Scheme Shell) which can be found at http://www.scsh.net/
or simply, if you are using Ubuntu, by giving a shell-command:
sudo apt-get install scsh

The code given here has been tested to work at least under the version 0.6.7,
released May 16, 2006, but it is known to have worked also under earlier
releases, such as 0.6.1.

Then get Wandy Sae-Tan's and Olin Shiver's FPS (Functional PostScript)
library from http://www.scsh.net/resources/fps.html
(This page is also archived as:
  http://web.archive.org/web/20080925094422/http://www.scsh.net/resources/fps.html
)

Specifically, the tar-ball of the library itself:
  http://ftp.scsh.net/pub/scsh/contrib/fps/fps-1.0.tar.gz

and the associated patch:
  http://ftp.scsh.net/pub/scsh/contrib/fps/fps-1.0-patch-for-scsh-0.5.3

(Neither the latter two files nor
 http://ftp.scsh.net/pub/scsh/0.6/scsh-0.6.7.tar.gz
are yet archived by Internet Archive as of today, June 17 2011,
but we are waiting...)

Unpack the library as:

  tar xvfz fps-1.0.tar.gz

and then apply the patch (staying in the same directory where you issued
the tar xvfz command, i.e. one directory above fps-1.0):

  patch -p0 < fps-1.0-patch-for-scsh-0.5.3

This should output the following four lines of text:
patching file fps-1.0/fps-examples.scm
patching file fps-1.0/fps.afm.scm
patching file fps-1.0/fps.glyph.scm
patching file fps-1.0/fps.scm

Unpack this shar-archive for example with command:

  unshar Catalan_Interpretations_Drawing_Routines_Package.shar.txt

and copy its contents to _THAT SAME fps-1.0 DIRECTORY_ (yeah!),
and then proceed as explained in the comments given at the
front of Catalan_Interpretations_FPS_drawing_routines.scm module.

If you encounter problems, please contact me at:

                               <my_firstname>.<my_surname>@gmail.com

                               Yours,

                               Antti Karttunen
                               Helsinki, June 17 2011.

