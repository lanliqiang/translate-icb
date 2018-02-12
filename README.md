# Emacs interface to ICB Translate

## Summary

This library allows to translate the strings using ICB Translate
service.

## Installation

#### Manual installation

Assuming that the file `translate-icb.el` is somewhere on the
load path, add the following lines to your `.emacs` file:

(load-library "translate-icb")

The command (global-set-key "\C-c\ \C-f" 'translate-icb) of library
set the binding of key ("\C-c\ \C-f") to 'translate-icb' function.
Invoking the function `translate-icb` to translate the word at point 
from en to cn or cn to en, and shows a buffer with available translations of the text. 

#### FAQ

Find load path:
"C+x b"(switch-to-buffer)
Display buffer BUFFER-OR-NAME in the selected window.
Select "*scratch*" buffer.
Insert lisp expression

(print load-path)

as you type expression into the buffer followed 
by "C-j" (eval-print-last-sexp) after (print load-path) expression, 
the buffer records the load-path value;
