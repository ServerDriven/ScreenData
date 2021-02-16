### Button
```
Button {
	id: String?

	title: String

	actionID: String?
	destination: Destination?

	style: Style?

	type: ViewType = .button
}
```

### JSON Example
```
{
  "destination": {
	"type": "screen",
	"toID": "detail"
  },
  "title": "Some Title with an Action",
  "style": {
	"padding": 8,
	"foregroundColor": {
	  "red": 1,
	  "alpha": 1,
	  "blue": 0,
	  "green": 0
	},
	"isHidden": true,
	"cornerRadius": 8,
	"backgroundColor": {
	  "red": 0.314,
	  "alpha": 1,
	  "blue": 0.314,
	  "green": 0.314
	}
  },
  "actionID": "0001"
}
```