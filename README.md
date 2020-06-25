gpp-macros
==========

Macros for use with [gpp](http://en.nothingisreal.com/wiki/GPP),
a general purpose macro preprocessor. GPP is a program that
allows the user to specify macros with arguments using a customizable
syntax. I use it to define LaTeX-like macros which are turned into
RTF code. For example this will define a macro called `\Huge` that
will create 48 point text:

    \define{\Huge}{{\fs96 #1}}

and it can be called in the RTF document like this:

    This text is \Huge{huge}.

I am using MS Windows so I might process my file like this

    c:\gpp\gpp.exe -o output.rtf -T input.rtf

where the `-T` specifies a Tex-like syntax.
