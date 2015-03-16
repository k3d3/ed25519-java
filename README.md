Don't use this!
===============

This library was the first implementation of ed25519 in Java, and I highly recommend you don't use this for anything serious. It uses BigInteger for everything and is therefore extremely slow (takes 5 seconds to sign a message) and is also not secure against side-channel or timing attacks.

Instead, you should use the [updated version by str4d](https://github.com/str4d/ed25519-java) which is not only much faster, but also more secure than this code.

Consider this code to be legacy.

ed25519-java
============

Ed25519 ported to Java

This class was ported from the Python Ed25519 reference implementation, located at http://ed25519.cr.yp.to/python/ed25519.py

It is not meant to be a proper OOP Java class, but rather a (mostly) direct translation from the Python code.

Compile and run test.java, and compare the output to validtest.txt - if it matches, you have a working Ed25519 library.

This code is released to the public domain and can be used for any purpose.
