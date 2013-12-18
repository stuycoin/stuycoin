Stuycoin
========

- Copyright (c) 2009-2013 Bitcoin Developers
- Copyright (c) 2011-2013 Litecoin Developers
- Copyright (c) 2013 Stuycoin Developers

What is Stuycoin?
-----------------

Stuycoin is a fork of Litecoin v0.8.6.1, itself a fork of Bitcoin using scrypt
as a proof-of-work algorithm.
 - 2.5 minute block targets
 - subsidy halves in 840k blocks (~4 years)
 - ~84 million total coins

The rest is the same as Litecoin and Bitcoin.
 - 50 coins per block
 - 2016 blocks to retarget difficulty

License
-------

Stuycoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers are requested to work in forks or separate branches, then submit
pull requests when they think their feature or bug fix is ready.

The `master` branch is a relatively stable integration branch.
[Tags](https://github.com/stuycoin/stuycoin/tags) are created to indicate new
official, stable release versions of Litecoin.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./litecoin-qt_test
