# Lab Wins & Understanding
I think the main thing I used in the lab was the 'curiosity question' concept and practicing my questions for things I had no idea if it would even work. For example, I knew how the psuedo classes should work, but my question was, to narrow it down, can I put two psuedo classes in one selector to further target? I tested it out and it worked immediately so that was really exciting. From there, it became really easy to target exactly what I wanted without accidentally styling someting else.

Although I was able to use the nth and first/last child psuedo classing, just having to add one a color or font-family was simple, but when I get into other use cases for it such as 'order' in relation to flexbox, I know that's something I will need to work on.

# Deeper Learning Debug
The spacing in the paragraph elements on the page is being caused by the margin added to the .task-box class. Since margin is between elements, and certain areas have a mark, bold, or italic inline element, the margin is being added there as well.

To solve this, I tried out .task-box p :not(p) {
    margin: 0px;
}.
Instead of creating a line for each inline element, I made my selector look at p and choose anything that was not the paragraph element. Then I made those margin 0px.