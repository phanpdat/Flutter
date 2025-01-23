import 'package:flutter/material.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  void printOntap() {
    // ignore: avoid_print
    print("Hello World");
  }

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      home: Scaffold(
        body: GestureDetector(
          onTap: () {
            printOntap();
          },
          child: Center(
            child: Container(
              color: Colors.deepPurple,
              width: 300,
              height: 300,
              child: Center(
                child: Text(
                  "ontap",
                  style: TextStyle(
                    fontSize: 30,
                  ),
                ),
              ),
            ),
          ),
        ),
      ),
    );
  }
}
