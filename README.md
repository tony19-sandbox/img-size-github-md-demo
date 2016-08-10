Inspired by question at:
http://stackoverflow.com/questions/14675913/how-to-change-image-size-markdown

|Source|Code   |Effect         |Pass/Fail|
|--- |---    |---            |--- |
|[:link:](http://stackoverflow.com/a/21242579/6277151)|`![](URL =200x100)`|![](http://www.sheawong.com/wp-content/uploads/2013/08/keephatin.gif =200x100)|:x:|
|[:link:](http://stackoverflow.com/a/21242579/6277151)|`![](URL =200x)`|![](http://www.sheawong.com/wp-content/uploads/2013/08/keephatin.gif =200x)|:x:|
|[:link:](http://stackoverflow.com/a/14747656/6277151)|`<img src="URL" style="width: 200px;"/>`|<img src="http://www.sheawong.com/wp-content/uploads/2013/08/keephatin.gif" style="width: 200px;"/>|:x:|
|[:link:](http://stackoverflow.com/a/21972032/6277151)|`<img src="URL" width="200" height="200" />`|<img src="http://www.sheawong.com/wp-content/uploads/2013/08/keephatin.gif" width="200" height="200" />|:white_check_mark:|
|[:link:](http://stackoverflow.com/a/33566654/6277151)|`<img src="URL" width="200">`|<img src="http://www.sheawong.com/wp-content/uploads/2013/08/keephatin.gif" width="200">|:white_check_mark:|
|[:link:](http://stackoverflow.com/a/30973855/6277151)|`![smiley](URL){:height="200px" width="200px"}`|![smiley](http://www.sheawong.com/wp-content/uploads/2013/08/keephatin.gif){:height="200px" width="200px"}|:x:|
|[:link:](https://github.com/tiimgreen/github-cheat-sheet#imagesgifs)|`[[ URL | width = 200px ]]`|(see [Wiki](https://github.com/tony19-sandbox/img-size-github-md-demo/wiki) for demo)|`Wiki`: :white_check_mark: `README`::x:|

This GitHub Markdown syntax:
```
[[ URL | width = 200px ]]
```

doesn't render properly in the `README` for some reason (issue reported). It renders plaintext:

[[ https://github.com/tiimgreen/github-cheat-sheet#imagesgifs | width = 200px ]]

