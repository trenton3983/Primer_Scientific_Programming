# Primer_Scientific_Programming

This repository contains resources for the Springer book

<!--
Automatically generated HTML file from DocOnce source
(https://github.com/hplgit/doconce/)
-->
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<meta name="generator" content="DocOnce: https://github.com/hplgit/doconce/" />
<meta name="description" content="Resources for A Primer on Scientific Programming with Python">
</head>

<!-- tocinfo
{'highest level': 1,
 'sections': [(' The 4th edition ', 1, None, '___sec0'),
              (' All programs from the book ', 2, None, '___sec1'),
              (' Erratalist ', 2, None, '___sec2'),
              (' Software installation ', 2, None, '___sec3'),
              (' Software installation on Ubuntu ', 2, None, '___sec4'),
              (' Slides ', 2, None, '___sec5'),
              (' The 3rd edition ', 1, None, '___sec6'),
              (' All programs from the book ', 2, None, '___sec7'),
              (' Software installation ', 2, None, '___sec8'),
              (' Software installation on Ubuntu ', 2, None, '___sec9'),
              (' Erratalist ', 2, None, '___sec10'),
              (' Slides ', 2, None, '___sec11'),
              (' The 1st and 2nd edition ', 1, None, '___sec12')]}
end of tocinfo -->

<body>

    
<!-- ------------------- main content ---------------------- -->



<center><h1>Resources for A Primer on Scientific Programming with Python</h1></center>  <!-- document title -->

<p>
<!-- author(s): Hans Petter Langtangen -->

<center>
<b>Hans Petter Langtangen</b>  (<tt>hpl at simula.no</tt>)
</center>


<p>
<!-- institution(s) -->

<h1 id="___sec0">The 4th edition </h1>

<p>
<a href="http://www.amazon.com/Scientific-Programming-Computational-Science-Engineering/dp/3642549586/ref=sr_1_2?s=books&ie=UTF8&qid=1407225588&sr=1-2&keywords=langtangen"><img border="0" width="130" src="figs/Primer4th_pic.jpg"></a>

<h2 id="___sec1">All programs from the book </h2>

<p>
On Unix/Linux or Mac, download
the tarfile <a href="book-examples-4th.tar.gz" target="_self"><tt>book-examples-4th.tar.gz</tt></a>
for the 4th edition and pack it out by

<p>

<!-- code=text (!bc sys) typeset with pygments style "default" -->
<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%">tar xvzf book-examples-4th.tar.gz
</pre></div>
<p>
On Windows, download <a href="book-examples-4th.zip" target="_self"><tt>book-examples-4th.zip</tt></a>
for the 4th edition and pack it out by

<p>

<!-- code=text (!bc sys) typeset with pygments style "default" -->
<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%">unzip book-examples-4th.zip
</pre></div>
<p>
or double click on the file icon.

<p>
The result is a folder (directory)
tree <code>src</code> with subfolders containing
the program examples for different chapters in the book
(<code>formulas</code>, <code>looplist</code>, etc., as explained in the introduction to
each chapter).

<p>
You can also directly access the latest version of the example
files at <a href="https://github.com/hplgit/scipro-primer" target="_self">GitHub</a>, see
the <a href="https://github.com/hplgit/scipro-primer/tree/master/src" target="_self">src</a>
directory (to download a file, click the <em>Raw</em> button on the right first
to get the pure text file in the browser and then right-click to download).
To copy the whole repository to your computer, run

<p>

<!-- code=text (!bc sys) typeset with pygments style "default" -->
<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%">git clone https://github.com/hplgit/scipro-primer.git
</pre></div>

<h2 id="___sec2">Erratalist </h2>

<p>
Here is a <a href="erratalist4th.pdf" target="_self">PDF file</a> or an <a href="erratalist4th.html" target="_self">HTML file</a> with an errata list for the
4th edition of the book. If you find any typo or error, please
report it to <a href="mailto:hpl@simula.no" target="_self">the author</a>.

<h2 id="___sec3">Software installation </h2>

<p>
There are several ways to access Python, either on your computer or
in the cloud. <a href="http://hplgit.github.io/edu/accesspy/accesspy_primer4.html" target="_self">Appendix H.1</a> in the book gives an overview of
recommended technologies and how to use them to get the software you need
for working with the book.

<p>
<b>SciTools.</b>
The package SciTools is freqently referred to and used in the book.
You may want to install SciTools directly from its Mercurial version control
repository. This makes it easy to upgrade the package at any time.
SciTools is hosted at <a href="https://github.com/hplgit/scitools/" target="_self">Googlecode</a>.
Make sure you have the Mercurial (<tt>hg</tt>) version control system
on your computer (if not, do <code>sudo pip install mercurial</code> on Linux or Mac,
and <code>pip install mercurial</code> in a Windows Command Prompt or Power Shell window).
Get the SciTools source code and install it by

<p>

<!-- code=text (!bc sys) typeset with pygments style "default" -->
<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%">git clone https://github.com/hplgit/scitools.git
cd scitools
sudo python setup.py install
</pre></div>
<p>
Whenever you want to upgrade the package, just go to the <code>scitools</code>
folder and run the commands

<p>

<!-- code=text (!bc sys) typeset with pygments style "default" -->
<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%">git pull origin master
sudo python setup.py install
</pre></div>

<h2 id="___sec4">Software installation on Ubuntu </h2>

<p>
If you have an Ubuntu installation, Python is already there. The minimum
extra packages are installed by this command:

<p>

<!-- code=text (!bc sys) typeset with pygments style "default" -->
<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%">sudo apt-get install python-matplotlib python-scipy python-gnuplot gnuplot gnuplot-x11 python-scitools
</pre></div>
<p>
A comprehensive installation with lots of useful packages can be
performed by a <a href="https://raw.github.com/hplgit/vagrantbox/master/doc/src/vagrant/src-vagrant/install_rich.sh" target="_self">Bash script</a>. Download this file (<code>install_rich.sh</code>) and run it by <code>bash install_rich.sh</code>.

<h2 id="___sec5">Slides </h2>

<p>
There is a <a href="slides/index.html" target="_self">slide collection</a>
from lectures based on the book.

<p>
<hr>

<h1 id="___sec6">The 3rd edition </h1>

<p>
<a href="http://www.amazon.com/Scientific-Programming-Computational-Science-Engineering/dp/3642302920/ref=sr_1_4?ie=UTF8&qid=1344338912&sr=8-4&keywords=langtangen+primer"><img border="0" width="130" src="figs/Primer_pic.jpg"></a>

<h2 id="___sec7">All programs from the book </h2>

<p>
On Unix/Linux or Mac, download
the tarfile <a href="book-examples-3rd.tar.gz" target="_self"><tt>book-examples-3rd.tar.gz</tt></a>
for the 3rd edition and pack it out by

<p>

<!-- code=text (!bc sys) typeset with pygments style "default" -->
<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%">tar xvzf book-examples-3rd.tar.gz
</pre></div>
<p>
On Windows, download <a href="book-examples-3rd.zip" target="_self"><tt>book-examples-3rd.zip</tt></a>
for the 3rd edition and pack it out by

<p>

<!-- code=text (!bc sys) typeset with pygments style "default" -->
<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%">unzip book-examples-3rd.zip
</pre></div>
<p>
or double click on the file icon.

<p>
The result is a folder (directory)
tree <code>src</code> with subfolders containing
the program examples for different chapters in the book
(<code>formulas</code>, <code>looplist</code>, etc., as explained in the introduction to
each chapter).

<p>
You can also directly access the latest version of the example
files at <a href="https://github.com/hplgit/scipro-primer" target="_self">GitHub</a>, see
the <a href="https://github.com/hplgit/scipro-primer/tree/master/src-3rd" target="_self">src-3rd</a>
directory (to download a file, click the <em>Raw</em> button on the right first
to get the pure text file in the browser and then right-click to download).
To copy the whole repository to your computer, run

<p>

<!-- code=text (!bc sys) typeset with pygments style "default" -->
<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%">git clone https://github.com/hplgit/scipro-primer.git
</pre></div>

<h2 id="___sec8">Software installation </h2>

<p>
The <a href="install.html" target="_self">old software description</a> is now outdated, so we
refer to the <a href="http://hplgit.github.io/edu/accesspy/accesspy_primer4.html" target="_self">new one</a> that appears in the 4th edition.

<p>
You may want to install SciTools directly from its Mercurial version control
repository. This makes it easy to upgrade the package at any time.
SciTools is hosted at <a href="https://github.com/hplgit/scitools/" target="_self">Googlecode</a>.
Make sure you have the Mercurial (<tt>hg</tt>) version control system
on your computer (if not, do <code>sudo pip install mercurial</code> on Linux or Mac,
and <code>pip install mercurial</code> in a Windows Command Prompt or Power Shell window).
Get the SciTools source code and install it by

<p>

<!-- code=text (!bc sys) typeset with pygments style "default" -->
<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%">hg clone https://langtangen@code.google.com/p/scitools/
cd scitools
sudo python setup.py install
</pre></div>
<p>
Whenever you want to upgrade the package, just go to the <code>scitools</code>
folder and run the commands

<p>

<!-- code=text (!bc sys) typeset with pygments style "default" -->
<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%">hg pull
hg update
sudo python setup.py install
</pre></div>

<h2 id="___sec9">Software installation on Ubuntu </h2>

<p>
If you have an Ubuntu installation, Python is already there. The minimum
extra packages are installed by this command:

<p>

<!-- code=text (!bc sys) typeset with pygments style "default" -->
<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%">sudo apt-get install python-matplotlib python-scipy python-gnuplot gnuplot gnuplot-x11 python-scitools
</pre></div>
<p>
A comprehensive installation with lots of useful packages can be
performed by a <a href="https://raw.github.com/hplgit/vagrantbox/master/doc/src/vagrant/src-vagrant/install_rich.sh" target="_self">Bash script</a>. Download this file (<code>install_rich.sh</code>) and run it by <code>bash install_rich.sh</code>.

<h2 id="___sec10">Erratalist </h2>

<p>
There is a <a href="erratalist3rd.pdf" target="_self">PDF file</a> with an errata list for the
3rd edition of the book.

<h2 id="___sec11">Slides </h2>

<p>
There is a <a href="http://www.ifi.uio.no/~inf1100/slides" target="_self">slide collection</a>
from lectures based on the 3rd edition of the book.

<h1 id="___sec12">The 1st and 2nd edition </h1>

<p>
The resource page for the first two editions is located
<a href="http://vefur.simula.no/intro-programming" target="_self">elsewhere</a>.

<!-- ------------------- end of main content --------------- -->


</body>
</html>
