import 'package:flutter/material.dart';

class CounterPage extends StatefulWidget {
  const CounterPage({super.key});

  @override
  State<CounterPage> createState() => _CounterPageState();
}

class _CounterPageState extends State<CounterPage> {
  int counter = 0;

  void updatecounter() {
    setState(() {
      counter++;
    });
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        backgroundColor: Colors.blueAccent,
        title: Text("Counter App"),
      ),
      body: Column(
        mainAxisAlignment: MainAxisAlignment.center,
        children: [
          Center(child: Text("you have pushed the button this many time !!")),
          Text(
            counter.toString(),
            style: TextStyle(
              fontSize: 40,
            ),
          ),
          ElevatedButton(
            onPressed: updatecounter,
            style: ElevatedButton.styleFrom(
              backgroundColor: Colors.green,
            ),
            child: Text("On tap"),
          ),
        ],
      ),
    );
  }
}
