[ArrayBox.dev](https://arraybox.dev) is an open-source online all-in-one REPL for six array languages, and the winner of the non-APL category of the 2026 Dyalog APL Forge competition.

It brings the six array languages into one REPL, sharing consistent editing tools, documentation, and keyboard support. You can write and evaluate code, translate basic expressions between languages, look up primitives without leaving the editor, and share what you've written with a permalink.

The Dyalog '26 presentation gives a tour of the website and its features.

[▶ Watch the presentation on YouTube](https://youtu.be/MO1sk4W8H5Q)

## How I fell in love with APL

In 2019, [Functional Geekery](https://dev.to/functional-geekery) introduced me to Dyalog APL and [TryAPL](https://tryapl.org/). That December, I finally sat down to experiment with the language.

The first primitive I tried was iota, `⍳`, which I was familiar with from C++'s `std::iota`. Then I tried plus reduce and plus scan:

| Expression | Result |
| --- | --- |
| `⍳5` | `1 2 3 4 5` |
| `+/⍳5` | `15` |
| `+\⍳5` | `1 3 6 10 15` |

The third expression blew my mind. Reduce gives the final accumulated result; scan gives all the intermediate accumulated results. In APL, that relationship is right there in the notation: `+/` and `+\`.

The corresponding C++ algorithms, `std::reduce` and `std::partial_sum`, hadn't made that relationship obvious to me. Playing with APL did. Reduce and scan are *twin algorithms*.

That discovery led to months of exploring array languages and their literature. Finding a dedicated glyph for rotate only added to my excitement. These languages put algorithms at the center of their notation, and studying them can change how you approach problems in any language.

The longer version of that story is in my 2022 talk [The Twin Algorithms](https://www.youtube.com/watch?v=NiferfBvN3s). I give the longer version of how I fell in love with APL and array languages starting at [8m51s](https://www.youtube.com/watch?v=NiferfBvN3s&t=531s) of that talk. ArrayBox makes it easier to continue that kind of exploration across languages.

![Iota, plus reduce, and plus scan in ArrayBox, with the scan result displayed below the code.]({{ site.baseurl }}/images/arraybox/reduce-and-scan.png)

## Why ArrayBox.dev?

Moving between the array languages' online REPLs is irritating. Some have syntax highlighting, some have automatic formatting, and some have dark mode. Some have none of the above.

ArrayBox brings these features into a shared environment, along with tools such as inline documentation. Put the cursor beside a primitive, press F1, and see what it does without leaving the code. Switching languages keeps those tools within reach.

Below is a screenshot of ArrayBox's help menu, showing the available shortcuts. For the rest of the article, we will highlight some of the features in more detail.

![ArrayBox's help menu showing shortcuts for evaluating code, switching languages, opening the keyboard, searching primitives, sharing links, and formatting.]({{ site.baseurl }}/images/arraybox/help-and-shortcuts.png)

## Six array languages in one editor

ArrayBox supports **Dyalog APL, BQN, Uiua, J, Kap, and TinyAPL**. Press **Ctrl + ↑** or **Ctrl + ↓** to cycle between them, or **Ctrl + P** to open the language picker.

The editor stays familiar as you switch. You have syntax highlighting, formatting, a dark background, and aligned comments, along with the documentation and primitive input tools for the selected language. That makes it easy to try an idea in a language you know and then explore how another language expresses it.

A GitHub Action checks daily for interpreter updates and opens issues and pull requests when new versions are available. This helps keep the REPL current, including beta releases.

![The ArrayBox language picker showing Dyalog APL, BQN, Uiua, J, Kap, and TinyAPL with their interpreter versions.]({{ site.baseurl }}/images/arraybox/six-languages.png)

## Translating between languages

Switching languages can also translate basic primitives and expressions.

For example, start with APL's `⍳5` and switch languages to see the corresponding expression.

Another example is reversing a literal array. When you switch languages, ArrayBox can translate the reverse primitive and adjust the notation used to write the array itself.

![Reversing the array 1 2 3 4 5 in Dyalog APL, producing 5 4 3 2 1.]({{ site.baseurl }}/images/arraybox/translation-apl.png)

*The expression in Dyalog APL.*

![The same reverse expression after switching to BQN, with translated array notation and the same result.]({{ site.baseurl }}/images/arraybox/translation-bqn.png)

*After switching to BQN, the array notation changes and the result stays the same.*

This is useful for learning the vocabulary of another language or comparing how a simple operation is expressed. More involved programs still need adaptation, particularly where indexing conventions and function composition differ. You can make those changes and test them in the same editor.

## Inline documentation

Put the cursor immediately to the left of a primitive and press **F1** to show its documentation inline. Press F1 again to close it.

You can read a description and an example while keeping the expression you're working on in view. The presentation demonstrates this with Dyalog's behind operator, `⍛`, looking up its behavior while building an expression.

![Inline documentation for Dyalog's behind operator beside the expression being evaluated, including its description, an example, and a link to the full documentation.]({{ site.baseurl }}/images/arraybox/inline-documentation.png)

Documentation is also available through the keyboard overlay. When a search narrows to a single primitive, its documentation appears alongside it. Pressing F1 in that view opens the full documentation page if you want more detail.

## Searchable keyboards and primitive input

Press **Ctrl + K** to open the keyboard overlay. For Dyalog APL, BQN, Kap, and TinyAPL, it shows syntax highlighted glyph mappings for a QWERTY keyboard. You can switch languages while the overlay is open to compare their mappings.

J uses ASCII notation, and Uiua lets you enter primitives by typing prefixes of their names, so those views show the primitive collections instead of keyboard mappings.

![The syntax highlighted Dyalog APL keyboard overlay, showing glyphs and their QWERTY key mappings.]({{ site.baseurl }}/images/arraybox/searchable-keyboard.png)

You can also type in the overlay to fuzzy search primitive names. For example, searching for a unique or deduplicate operation helps you find the matching primitives and inspect their documentation.

If you already know what operation you want but haven't memorized its key mapping, **Ctrl + Space** opens primitive search directly in the editor. Search by the primitive's documented name and insert the glyph. For example, APL's `⍳` is listed as *Index Generator*.

![Primitive search for "index" showing matching APL primitives, their names, and the keyboard shortcuts used to enter them.]({{ site.baseurl }}/images/arraybox/primitive-search.png)

## Editing and evaluating code

ArrayBox supports multiline code, evaluating a selection, and formatting without evaluation. Useful shortcuts include:

| Shortcut | Action |
| --- | --- |
| Enter | Evaluate code |
| Shift + Enter | Evaluate a selection, or insert a newline when nothing is selected |
| Ctrl + F | Format code without evaluating it |
| Ctrl + / | Comment or uncomment a line |
| Ctrl + Shift + ↑ / ↓ | Add a cursor above or below |

Multiple cursors let you make the same edit on several lines at once. There is also a shift-edit feature for changing matching occurrences of a string together, which gives you a lightweight find and replace workflow.

![Three cursors selecting the same glyph across separate lines of APL code, with aligned comments and an evaluation result.]({{ site.baseurl }}/images/arraybox/multiple-cursors.png)

For tacit expressions, the train tree helps you inspect how the functions group together. The presentation uses this view to explore composition, which is particularly helpful when moving between languages with different tacit models.

![ArrayBox's tree view showing how plus reduce, divide, and tally form the APL mean function.]({{ site.baseurl }}/images/arraybox/evaluation-tree.png)

Press **Ctrl + H** at any point to see the help menu and the available shortcuts.

## Sharing an expression

Once you have something you'd like to share, **Ctrl + L** creates a permalink and copies the URL. You can use it in a social post, send it to someone, or include it in a presentation so others can open the example themselves.

An empty editor can also share the selected language or its keyboard overlay, such as [this BQN keyboard](https://arraybox.dev/?kb=bqn).

You can [try ArrayBox.dev here](https://arraybox.dev) and follow along with the video, from experimenting with a primitive to comparing languages and sharing an expression.

## A live coding example

The presentation closes with the [Largest Interval problem from The Weekly Challenge 400](https://theweeklychallenge.org/blog/perl-weekly-challenge-400/#task-1-largest-interval): remove integers with repeated digits and find the largest gap between the remaining values. The walkthrough builds and debugs a solution in Dyalog APL, then adapts it to Kap and TinyAPL. It's a chance to see the documentation, editing tools, and language switching in action on the same problem.

![ArrayBox running the Dyalog APL Largest Interval solution and displaying the five results: 2, 4, 11, 105, and 105.]({{ site.baseurl }}/images/arraybox/largest-interval.png)

I wasn't able to attend the Dyalog '26 conference in person this year, but I hope to attend in the future and see you there!
