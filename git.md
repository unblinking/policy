# Git  

## .gitattributes  

To deal with line endings, use a ```.gitattributes``` file configured so that Git will always convert line endings to LF on checkout. This keeps LF endings, even on Windows.

[github.com dealing with line endings](https://help.github.com/articles/dealing-with-line-endings/)  

```
# Set the default behavior, in case people don't have core.autocrlf set.
* text eol=lf
```
