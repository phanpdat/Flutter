import 'package:flutter/material.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      home: Scaffold(
        backgroundColor: const Color.fromARGB(255, 184, 203, 203),

        //                     App bar

        appBar: AppBar(
          backgroundColor: Colors.deepPurpleAccent,
          title: Center(

              //                Text

              child: Text(
            "My App",
            style: TextStyle(
              color: Colors.amberAccent,
              fontSize: 30,
              fontWeight: FontWeight.bold,
            ),
          )),
        ),
        body: Center(
          //                  Container

          child: Container(
            //padding:EdgeInsets.symmetric(horizontal: 20 , vertical: 20),
            width: 200,
            height: 200,
            // ignore: sort_child_properties_last
            child: Column(
              mainAxisAlignment: MainAxisAlignment.center,
              children: [
                Center(child: Text("HiHi!!!")),

                //              ICONS

                Icon(
                  Icons.menu,
                  color: Colors.amberAccent,
                  size: 40,
                  textDirection: TextDirection.ltr,
                ),
              ],
            ),
            decoration: BoxDecoration(
              borderRadius: BorderRadius.circular(20),
              color: Colors.blue,
            ),
          ),
        ),
      ),
    );
  }
}
