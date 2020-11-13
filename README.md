# ScreenData
A Data Model structure for displaying UI Screens


## Model POC

### Screen
```
Screen {
        id: String? // UUID

	title: String
	subtitle: String?
	
	backgroundColor: Color
	
	headerView: View?
	views: [View]
	footerView: View?
}
```

### ViewDirectionAxis
```
enum ViewDirectionAxis {
	case vertical
	case horizontal
}
```

### View
```
View {
	title: String
	subtitle: String?
	
	type: ViewType
	
	image: Image?
	
	destination: Screen?
	axis: ViewDirectionAxis
	
	views: [View]
}
```

### ViewType
```
enum ViewType {
	case label
	case image
	case labeledImage
	case container
}
```

### Views

#### Label
```
Label {
	title: String
	subtitle: String?
	
	type: ViewType = .label
	
	destination: Screen?
}
```

#### Image
```
Image {
	image: Image
	
	type: ViewType = .image
	
	destination: Screen?
}
```

#### LabeledImage
```
LabeledImage {
	title: String
	subtitle: String?
	image: Image
	
	type: ViewType = .labeledImage
	
	destination: Screen?
}
```

#### ContainerView
```
ContainerView {
	type: ViewType = .container

	axis: ViewDirectionAxis

	views: [View]
}
```

#### DestinationType
```
DestinationType {
	case screen
	case url
	case deepLink
}
```

#### ScreenDestination
```
ScreenDestination {
	screenID: String
	type: DesitinationType = .screen
}
```

#### URLDestination
```
URLDestination {
	url: String
	type: DestinationType = .url
}
```

#### DeepLinkDestination
```
DeepLinkDestination {
	screens: [DeepLinkScreen]
	type: DestinationType = .deepLink
}
```

##### DeepLinkScreen
```
DeepLinkScreen {
	screenID: String
	order: Int
}
```
