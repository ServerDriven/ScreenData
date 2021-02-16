### Text
```
Text {
	id: String?

	title: String

	style: Style?

	type: ViewType = .text
}
```

### JSON Example
```
{
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
```