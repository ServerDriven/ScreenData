### Image
```
Image {
	id: String?

	url: String
	aspectScale: ImageAspectScale

	style: Style?

	destination: Destination?

	type: ViewType = .image
}
```

### JSON Example
```
{
  "url": "(...).png",
  "aspectScale": "fill",
  "style": {
	"isHidden": false,
	"height": 320,
	"cornerRadius": 0,
	"padding": 0
  }
}
```