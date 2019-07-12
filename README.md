## UILabel dynamic height & width using constraints:

http://stackoverflow.com/questions/34009311/autolayout-uilabel-not-resizing-properly-with-long-text/34009386#34009386

This behavior is supported with Auto-layout on. And by following these steps for the UILabels in question.

1. Set number of lines to '0' in the Utilities pane > Attributes inspector.

2. Right click the UILabel and Alt - control (Xcode 7.1 and above) drag to it's superview to set the leading, trailing, top and bottom margin.

3. For auto height and width you can set the priority of the constraint to level '<b>600</b>' with relation 'Greater than or Equal'.

Github example (I only use a different 'relation' for the bottom constraint in the following example. You could also choose to do this for a different constraint i.e. the trailing constraint): https://github.com/wojtekdmyszewicz/UILabel
