gpp-macros
==========

Macros for use with [gpp](http://en.nothingisreal.com/wiki/GPP),
a general purposes macro preprocessor. This is program that
allows the user to specify macros with arguments using a customizable
syntax. I use it to define LaTeX-like macros which are turned into
RTF code. For example this will make 48 point text:

    \define{\Huge}{{\fs96 #1}}

and it can be called in the RTF document like this:

    This text is \Huge{huge}.


