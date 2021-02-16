### Label
```
Label {
	id: String?

	title: String
	subtitle: String?

	font: FontType
	style: Style?

	destination: Destination?

	type: ViewType = .label
}
```

### JSON Example
```
{
  "title": "Home",
  "font": "title",
  "style": {
	"foregroundColor": {
	  "red": 1,
	  "alpha": 1,
	  "blue": 1,
	  "green": 1
	},
	"isHidden": false,
	"cornerRadius": 0,
	"padding": 8
  }
}
```