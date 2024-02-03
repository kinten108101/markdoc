# MarkDoc

A distributed system of note repositories / Zettelkastens.

For a brief history, refer to Various Zettelkasten's[^varzet].

## Repositories

These repositories are (in chronological order):

- Joplin: A Joplin repository with Dropbox backend managed by gb.lenguyen@gmail.com (Linked with Dropbox);
- BlackMountain: A Trello repository managed by kinten108101@protonmail.com (Linked with Atlassian);
- markdoc: Markdown files on local machine managed by kinten@Archio;
- engineeringWiki: An Obsidian repository managed by kinten@Archio;
- Gia Bảo's Notion: A Notion repository managed by gb.lenguyen@gmail.com (Linked with Google Account);
- Blobbook 0: A Le Hong Phong notebook;
- Blobbook 1: A Lazada notebook;
- Blobbook 2: A VNG notebook;
- Blobbook 3: A Blue Angel notebook;
- MarkDoc: A Bundled Notes repository managed by gb.lenguyen@gmail.com (Linked with Google Account);

Disconnected repositories:

- Firefly: A OneNote repository;
- Evernote;
- Bear;
- Werdsmith;
- Drafts;
- Google Keep;
- Simple Notes;
- Standard Notes;
- and many more lost to time...

## Naming system

MarkDoc uses a naming scheme that closely resembles the URI system with a `markdoc` protocol.

Or you can use the EBNF form below for the absolute path:

```
repository = 'engineeringWiki' | '"Gia Bảo's Notion"' | ...
item = ( 'markdoc:///' )? repository '/' (collection '/')* item '#' section
```

Some other rules:

- If item is a file, do not include file extension;
- Relative path is possible and is encouraged.

For example, to refer to the "In Future" section in the "Various Zettelkasten's" article in the engineeringWiki repository, write `engineeringWiki/Various Zettelkasten's#In Future`

[^varzet]: markdoc:///engineeringWiki/Various Zettelkasten's
