### ContainerView
```
ContainerView {
	id: String?

	isScrollable: Bool
	axis: ViewDirectionAxis
	views: [SomeView]

	style: Style?

	type: ViewType = .container
}
```


### JSON Example
```
{
  "id": "visit",
  "title": "Visit",
  "backgroundColor": {
	"red": 0,
	"alpha": 1,
	"blue": 0,
	"green": 0
  },
  "someView": {
	"type": "container",
	"someContainer": {
	  "axis": "vertical",
	  "style": {
		"padding": 0,
		"isHidden": false,
		"cornerRadius": 0
	  },
	  "isScrollable": true,
	  "views": [
		{
		  "type": "image",
		  "someImage": {
			"url": "https:(...).png",
			"aspectScale": "fill",
			"style": {
			  "isHidden": false,
			  "height": 320,
			  "cornerRadius": 0,
			  "padding": 0
			}
		  }
		}
	  ]
	}
  }
}
```