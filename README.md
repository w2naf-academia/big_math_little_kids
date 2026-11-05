# Big Math, Little Kids

Printable worksheets that teach big mathematical ideas to second graders: differential
equations, related rates, imaginary numbers and Euler's equation. Each one tells a story and
uses counting, pictures and hands-on activities in place of algebra. Every worksheet ends with an
answer key on its own page.

## Worksheets

Listed in teaching order. The last three build up to Euler's equation.

| Worksheet | Big idea | PDF |
| --- | --- | --- |
| **The Cookie Countdown** | Rates, a first differential equation (dC/dt = −20), and related rates through chocolate chips | [cookie_countdown.pdf](worksheets/cookie_countdown/cookie_countdown.pdf) |
| **The Count's Square Cookies** | Squares and square roots with cookie trays, why (−3) × (−3) = 9, and why j = +√−1: the turn that, done twice, turns you around. Snuffy, Big Bird's "imaginary" friend, lives at j | [count_square_cookies.pdf](worksheets/count_square_cookies/count_square_cookies.pdf) |
| **Cookie Monster's Growing Cookie Jar** | Where e comes from: a jar that grows in more and smaller steps (512, 576, 625, …) approaches e ≈ 2.72 jarfuls | [growing_cookie_jar.pdf](worksheets/growing_cookie_jar/growing_cookie_jar.pdf) |
| **The Cookie Circle** | Oscar's opposite trick (×(−1)) and Elmo's quarter turn (×*j*, the engineers' imaginary unit), Cookie Monster's cookie map (the complex plane), π from a cup and string, and Elmo's walk around a giant cookie: e<sup>jπ</sup> + 1 = 0 | [cookie_circle.pdf](worksheets/cookie_circle/cookie_circle.pdf) |

Print the PDFs directly. To leave the answers out of student copies, skip the last page.

The worksheets use Sesame Street characters by name only, for classroom use. They are not
affiliated with or endorsed by Sesame Workshop.

## Building from source

Each worksheet is a single LaTeX file with its figures drawn in TikZ. With TeX Live installed:

```bash
cd worksheets/cookie_countdown
pdflatex cookie_countdown.tex
pdflatex cookie_countdown.tex
```

## How these were made

The worksheets were written with AI assistance (Claude, by Anthropic) and reviewed by
Nathaniel A. Frissell (W2NAF), University of Scranton. Every AI-assisted session is recorded in
[`ai/ai_usage_log.md`](ai/ai_usage_log.md). The Cookie Countdown began as a Markdown draft, kept
in [`original_markdown_draft.md`](worksheets/cookie_countdown/original_markdown_draft.md); it was
moved to LaTeX because tables and positions broke when the Markdown was exported to PDF.

This repository follows the
[`ai_project_template`](https://github.com/w2naf-academia/ai_project_template) scaffold.
