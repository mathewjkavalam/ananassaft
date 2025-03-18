[Return Home](https://github.com/mathewjkavalam/ananassaft/blob/main/index.md)/[Go Back](https://github.com/mathewjkavalam/ananassaft/blob/main/obvious.md)
# How to end it well! Line endings and git
Line endings are invisible characters that are inserted when we press return key $$^{1}$$.
For example an online Latex document authoring platform, that I recently used $$^{2}$$ uses ```LF``` as the line ending character.
And Windows expects line endings to be ```CRLF```.

When I tried to version control those file I created using that platform, using git on my windows computer, I was greeted by this message
```
warning: in the working copy of 'xxx.tex', LF will be replaced by CRLF the next time Git touches it
```
Here git on sensing that the local environment is windows, proactively takes steps to make it compliant on a windows environment.
All was good if I am never returning back to that online platform. So to create a workflow which is circular,
the input expectation of the online latex platform should be the output given by git. So to configure this behaviour we can use
a file called ```.gitattributes``` $$^{3}$$ .
### References
* [1] [Github 2025](https://docs.github.com/en/get-started/git-basics/configuring-git-to-handle-line-endings#about-line-endings)
* [2] [Overleaf.com](https://www.overleaf.com/)
* [3] [Github 2025](https://docs.github.com/en/get-started/git-basics/configuring-git-to-handle-line-endings#about-line-endings)
