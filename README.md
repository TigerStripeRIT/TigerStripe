TigerStripe
================================

General Information (FaQ): https://tinyurl.com/y6r3oxys<br/>
Block Explorer: http://159.89.129.63:3001/

Copyright (c) 2009-2014 Bitcoin Developers<br/>
Copyright (c) 2011-2014 Litecoin Developers<br/>
Copyright (c) 2019 TigerStripe Developers<br/>

What is TigerStripe?
----------------

TigerStripe is a modified version of Litecoin created specifically for RIT students, faculty and alumni. The cryptocurrency uses scrypt as a proof-of-work algorithm and will remain fully decentralized, allowing safe, secure, fast, and efficient peer-to-peer transactions.
 - 2.5 minute block targets
 - subsidy halves in 840k blocks (~4 years)
 - ~84 million total coins
 - 50 coins per block
 - 2016 blocks to retarget difficulty

For more information, as well as an immediately useable, binary version of
the TigerStripe client sofware, check the "Releases" tab. You can view the full blockchain at http://159.89.129.63:3001/

License
-------

TigerStripe is released under the terms of the MIT license. See `COPYING` for more
information.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the TigerStripe
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/tigerstripe-project/tigerstripe/tags) are created
regularly to indicate new official, stable release versions of TigerStripe.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./tigerstripe-qt_test

