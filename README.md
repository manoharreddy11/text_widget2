import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('Text Widget Example'),
        ),
        body: Center(
          child: Text(
            'Hello World!',
            style: TextStyle(
              decoration: TextDecoration.lineThrough, 
              decorationColor: Colors.red,
              decorationStyle: TextDecorationStyle.solid,
              shadows: [
                Shadow(
                  color: Colors.black,
                  blurRadius: 2,
                  offset: Offset(2, 2),
                ),
              ], 
            ),
          ),
        ),
      ),
    );
  }
}
