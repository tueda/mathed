Math Editor
===========

Life is akin to an LMS where formulas cannot simply be copied and pasted;
they must be retyped relentlessly each time with a dedicated editor.
Both entail a continuous struggle.
While there is no ultimate solution for life,
we offer a practical solution to ease the struggles within *the LMS*.

The site provides an editor for writing text with LaTeX, which is then
translated into suitable HTML format for pasting into the LMS,
along with a rendering preview of the math using MathJax.

Unfortunately, when importing an Excel file listing questions in HTML format,
the clever LMS peremptorily removes all `span` tags.
To counteract this, you need to perform the following text replacements
in the HTML edit pane:

| Before replacement | After replacement |
| ---- | ---- |
| `\(` | `<span class="embedded-mathjax">\(` |
| `\)` | `\)</span>` |

Disclaimer: the code was written with GPT-4o.
