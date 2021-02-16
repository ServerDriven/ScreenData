### SomeView
```
SomeView {
	type: ViewType

	container: ContainerView?
	image: Image?
	label: Label?
	text: Text?
	button: Button?
	labeledImage: LabeledImage?
	customView: CustomView?
}
```

### Example JSON
```
{
  "type": "text",
  "someText": {
	"title": "...",
	"style": {
	  "foregroundColor": {
		"red": 1,
		"alpha": 1,
		"blue": 1,
		"green": 1
	  },
	  "isHidden": false,
	  "cornerRadius": 0,
	  "padding": 0
	}
  }
}
```