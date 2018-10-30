French and Bengali: `apertium-fra-ben`
===============================================================================

This is an Apertium language pair for translating between French and
Bengali. What you can use this language package for:

* Translating between French and Bengali
* Morphological analysis of French and Bengali
* Part-of-speech tagging of French and Bengali

For information on the latter two points, see subheading "For more
information" below.

Requirements
-------------------------------------------------------------------------------

You will need the following software installed:

* lttoolbox (>= 3.3.0)
* apertium (>= 3.3.0)
* vislcg3 (>= 0.9.9.10297)
* apertium-fra
* apertium-ben

If this does not make any sense, we recommend you look at: www.apertium.org.

Compiling
-------------------------------------------------------------------------------

Given the requirements being installed, you should be able to just run:

    $ ./configure
    $ make
    # make install

You can use `./autogen.sh` instead of `./configure` you're compiling from
source. If you installed any prerequisite language packages using a `--prefix`
to `./configure`, make sure to give the same `--prefix` to `./configure` here.

Testing
-------------------------------------------------------------------------------

If you are in the source directory after running make, the following
commands should work:

    $  echo "TODO test sentence 1" | apertium -d . fra-ben
    TODO test translated sentence 1

    $ echo "TODO test sentence 2" | apertium -d . ben-fra
    TODO test translated sentence 2

After installing somewhere in `$PATH`, you should be able to do e.g.

    $  echo "TODO test sentence 1" | apertium fra-ben
    TODO test translated sentence 1

Files and data
-------------------------------------------------------------------------------

* `apertium-fra-ben.fra-ben.dix`  - Bilingual dictionary
* `apertium-fra-ben.fra-ben.t1x`  - Chunking rules for translating into Bengali
* `apertium-fra-ben.ben-fra.t1x`  - Chunking rules for translating into French
* `apertium-fra-ben.fra-ben.t2x`  - Interchunk rules for translating into Bengali
* `apertium-fra-ben.ben-fra.t2x`  - Interchunk rules for translating into French
* `apertium-fra-ben.fra-ben.t3x`  - Postchunk rules for translating into Bengali
* `apertium-fra-ben.ben-fra.t3x`  - Postchunk rules for translating into French
* `apertium-fra-ben.fra-ben.lrx`  - Lexical selection rules for translating into Bengali
* `apertium-fra-ben.ben-fra.lrx`  - Lexical selection rules for translating into French
* `modes.xml`                     - Translation modes

For more information
-------------------------------------------------------------------------------

* http://wiki.apertium.org/wiki/Installation
* http://wiki.apertium.org/wiki/apertium-fra-ben
* http://wiki.apertium.org/wiki/Using_an_lttoolbox_dictionary

Help and support
-------------------------------------------------------------------------------

If you need help using this language pair or data, you can contact:

* Mailing list: apertium-stuff@lists.sourceforge.net
* IRC: `#apertium` on `irc.freenode.net`

See also the file AUTHORS included in this distribution.
