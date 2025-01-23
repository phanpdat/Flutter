// ignore_for_file: file_names
import 'package:flutter/material.dart';

class Firstpage extends StatelessWidget {
  const Firstpage({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        backgroundColor: Colors.deepPurple,
        title: Center(child: Text("My App")),
      ),
      body: Center(
        child: ElevatedButton(
          onPressed: () {
            // Navigator.push(
            //   context,
            //   MaterialPageRoute(builder: (context) => SecondPage()),
            // );
            Navigator.pushNamed(context, '/secondpage');
          },
          child: Text("secondPage"),
        ),
      ),
    );
  }
}
