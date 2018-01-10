# html-resume
A single-page résumé template done purely with HTML and CSS, which can be rendered into PDF through web browsers' print-to-PDF functionality, making a nice, sleek, professsional and ready-to-print résumé. See my living example at: https://mnjul.net/cv/resume.pdf

As the résumé is purely typeset with HTML and CSS, it's highly customizable (e.g. if you want an "objective" section, just copy-paste a few HTML elements) and does not require proprietary software. All you need is a text editor and a web browser (see compatibility section below). Oh, maybe some intermediate CSS knowledge. And, since it's open source with Apache License, you're allowed (and encouraged!) to create your own fine-tuned template and share with others.

Find the background story of this project at [my blog](https://blogs.purincess.tw/matrixblog/2016/04/typesetting-resume-with-html-and-css/).

# Compatibility and Known Issues/Limitations
* I have only tested this project on latest release version of Firefox (56 as of writing) and Google Chrome (61) on macOS 10.13 (High Sierra).
* It's my intention to support other browsers/platforms (like IE Edge on Windows?) as long as the browser sufficiently supports the required CSS features: ``calc()``, ``var()``, ``flexbox``, ...etc, and does not require (too many) dirty tricks. PRs or comments welcome!
* **No hyperlinking functionality in rendered PDF** as browers's print-to-PDF process is merely "flattening to digital paper".
* Other browser-specific hacks are as commented in the code.

# Fonts, Icon Fonts, and Dependencies
* [Open Sans](https://www.google.com/fonts/specimen/Open+Sans), [Source Code Pro](https://fonts.google.com/specimen/Source+Code+Pro) and [Source Sans Pro](https://www.google.com/fonts/specimen/Source+Sans+Pro) are used at various weights, but are not included in this repository. Please follow the links to download the fonts onto your computer.
* Icons from [Font Awesome](https://fortawesome.github.io/Font-Awesome/) are used and are incorporated as a git submodule in this repository.
* [Normalize.css](https://necolas.github.io/normalize.css/) is used and is incorporated as a git submodule in this repository.

# Paper Size/Orientation
* Currently letter portrait only. PRs welcome for other paper sizes --- especially A4!

# Actually Rendering the PDF
* Again...I've only tried on the said version of Firefox & Chrome, on macOS.
* Just open the HTML file with the browser. No need to serve the document from any kind of web server --- the ``file:///`` protocol should be good enough.
* On Firefox:
  * You probably need to remove any page margins in **about:config**.
  * Uncheck **Ignore Scaling and Shrink To Fit Page Width**.
  * Check **Print Background Colors**.
  * Clear out the headers and footers.
  * Save as PDF.
* On Google Chrome:
  * Set **Margin** to **None**.
  * Print **Background Graphics**.
  * Don't print headers and footers.
  * Save as PDF.

# Footnotes and License
* If you ever print out the rendered PDF, make sure texts are not clipped off, or items have not unexpectedly shrunk. Additionally, since the PDF has no margin outside the shaded sidebar, while most printers have no-print areas, the shaded sidebar probably won't fill up to the page's edge when printed.
* This project is licensed under the Apache License.
* PR, forks and other comments/suggestions are, as always, super welcome.
* Feel free to remove the ``#disclaimer`` block which links back to this repository --- but huge thanks if you decide to keep it.
* The layout/design was inspired by Paolo Zupin. Also, if anyone knows which link I should put under Mr. Zupin's name, please tell me!
