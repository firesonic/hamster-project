Coding Guidelines
=================

Licensing
---------
This project uses the MIT license. Please add this comment block at the top
of all source files. Replace <code>[first author]</code> with your own name.
Add additional authors (if any) as shown.

<pre>
/******************************************************************************
 * The MIT License (MIT)                                                      *
 *                                                                            *
 * Copyright (c) 2015 [first author], [second author], [third author],        *
 *                    [fourth author]                                         *
 *                                                                            *
 * Permission is hereby granted, free of charge, to any person obtaining a    *
 * copy of this software and associated documentation files (the "Software"), *
 * to deal in the Software without restriction, including without limitation  *
 * the rights to use, copy, modify, merge, publish, distribute, sublicense,   *
 * and/or sell copies of the Software, and to permit persons to whom the      *
 * Software is furnished to do so, subject to the following conditions:       *
 *                                                                            *
 * The above copyright notice and this permission notice shall be included in *
 * all copies or substantial portions of the Software.                        *
 *                                                                            *
 * THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR *
 * IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,   *
 * FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL    *
 * THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER *
 * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING    *
 * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER        *
 * DEALINGS IN THE SOFTWARE.                                                  *
 ******************************************************************************/
</pre>

Files and Directories
---------------------
- Keep all source and header files in <code>/src</code>.
- Header files have the extension <code>&ast;.h</code> for C headers, and
  <code>&ast;.hpp</code> for C++ headers.
- Source files have the extension <code>&ast;.c</code> for C code, and
  <code>&ast;.cpp</code> for C++ code.
- The <code>src.ino</code> is the only source file allowed to **not** follow the
  extension guidelines above since it's also the project file name. It's name is
  <code>src.ino</code> due to Arduino IDE enforcing this file to have the same
  name as the enclosing folder.
- Put all source and header files in the root directory. This is to avoid
  Arduino IDE getting confused over include directories more than anything.

Coding
------
- Please keep every line at *80 characters max* (unless it's significantly more
  readable otherwise). You can use the license header as a guideline (since it's
  exactly 80 visible characters wide.)
- If it's not too annoying, use one TAB character (not spaces) for *code block*
  indentation. Use SPACES whenever it's a *continuation* of a previous line.
  In any case, I'll fix this when merging on my end anyway.

  &ast;Yes, we're going against Arduino IDE's default in this case.

Other Notes
-----------
- Arduino automatically produces the main() function, function prototypes, and
  adds <code>#include &lt;Arduino.h&gt;</code> header line during the
  compilation process. This is why it seemingly works against C language
  standards. Just saying, since it probably won't work for any other source
  file.
