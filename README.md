*All files are based on QT project ones for clang.*

# qmake-zapcc
Files to support [zapcc](https://github.com/yrnkrn/zapcc) with qmake on linux and OS X (not tested).

# Working on

* Linux:
	* Qt 5.11.2 from self-installer
	* Ubuntu 18.04
	* zapcc commit https://github.com/yrnkrn/zapcc/commit/9bd04e7618bafaf6d938b0aed5837c1c5b312645
* OS X:
	* Not tested yet (report if you have tested it)

# How to use it?

Copy all three directories (**`common` must be merged and not replaced!**) into `YOUR_QT_INSTALLATION/QT_VERSION/gcc_64/mkspecs`. 
It is `~/.qt/5.11.2/gcc_64/mkspecs` in my case.

To use it, add `-spec linux-zapcc` (or `-spec macx-zapcc` on OS X) to `qmake` arguments, like

	qmake -spec linux-zapcc ..

# What if I have found a bug?

At first, make sure that `zapcc` and `zapcc++` are aviable in your `$PATH` (you can just type `zapcc` and get it is found).

If it's real bug, write to GitHub™ issues.
