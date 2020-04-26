# hackernews-threadlines

*Do you struggle to click the tiny [-] button? Are you tired of scrolling all the way back up when you want to collapse a thread? Do you lose track when you get deep in a comment thread? Then Hacker News threadlines are for you!*

A pure CSS solution means that you can get Reddit-style indentation threadlines just by copying a little code into your uBlock Origin configuration.

## Installation with uBlock Origin

Got to "My filters" on the uBlock Origin dashboard & copy in these four lines:

	news.ycombinator.com##.togg:before:style( content: ''; display: block; width: 1px; background-color: #828282; position: absolute; height: 10000px; padding: 8px; margin: 2px; background-clip: content-box; )
	news.ycombinator.com##.comment-tree:style( overflow: hidden; position: relative; )
	news.ycombinator.com##.default, .comment:style( background-color: #f6f6ef; box-shadow: 4px 4px 0 8px #f6f6ef; position: relative; width: 100%; )
	news.ycombinator.com##.comtr > td > table:style( width: 100%; )

## Installation with Stylus (user style)

The raw CSS is available in `hackernews-threadlines.css`. There's no official userstyle yet but if you're looking for one, your contribution is welcome!

## Contributing

Principles for this project are:

- make using hacker news easier;
- don't mess with the visual style (less is more); and
- dead simple installation for as many platforms as possible.

If you have tweaks you use on Hacker News, please create a PR or an issue. Feature requests are welcome!

Also, as mentioned above, creating a userstyle might be a good idea if someone is interested.
