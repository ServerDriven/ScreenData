### Screen
```
Screen {
	id: String?

	title: String
	subtitle: String?

	backgroundColor: Color

	headerView: SomeView?
	view: SomeView
	footerView: SomeView?
}
```

### JSON Example
```
{
  "title": "Uh oh!",
  "backgroundColor": {
	"red": 1,
	"alpha": 1,
	"blue": 1,
	"green": 1
  },
  "someView": {
	"type": "label",
	"someLabel": {
	  "title": "\/\/ TODO: This",
	  "font": "largeTitle",
	  "style": {
		"foregroundColor": {
		  "red": 0,
		  "alpha": 1,
		  "blue": 0,
		  "green": 0
		},
		"isHidden": false,
		"cornerRadius": 0,
		"padding": 0
	  }
	}
  }
}
```