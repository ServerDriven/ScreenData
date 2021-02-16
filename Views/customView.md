### CustomView
```
CustomView {
	id: String?

	title: String?
	subtitle: String?

	style: Style?

	image: Image?

	destination: Destination?
	axis: ViewDirectionAxis?

	views: [SomeView]?

	type: ViewType = .custom
}
```

### JSON Example
```
{
  "axis": "vertical",
  "id": "welcomeHeaderView",
  "title": "Welcome",
  "someImage": {
	"url": "(...).png",
	"aspectScale": "fill",
	"style": {
	  "isHidden": false,
	  "height": 320,
	  "cornerRadius": 0,
	  "padding": 0
	}
  },
  "view": []
}
```