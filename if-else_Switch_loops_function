import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

// ignore: must_be_immutable
class MyApp extends StatelessWidget {
  MyApp({super.key});
  int age = 18;
  String grade = "A";

  //                    I F - E L S E

  /*

  if () {

  } else {

  }

  */

  //                 S W I T C H - C A S E

  /*
  switch(condition){
  case a:  do something;
  break;
  case b:  do somthing;
  break;
  default: do something;
  }
  */

  //               F O R - L O O P

  /*
  for(int i=0;i<n;i++){
    do something
  }
  */

  //                  W H I L E

  /*
  while(condition){
    do something
  }
  */

  //          F U N C T I O N S( Hàm) / M E T H O D
  void greet() {
    // ignore: avoid_print
    print("good bye !!!");
  }

  void greetname(String name) {
    // ignore: avoid_print, prefer_interpolation_to_compose_strings
    print("Hello " + name);
  }

  int add(int a, int b) {
    return a + b;
  }

  @override
  Widget build(BuildContext context) {
    if (age == 18) {
      // ignore: avoid_print
      print("you are beeutiful");
    } else {
      // ignore: avoid_print
      print("you are not adult ");
    }

    if (grade == "A") {
      // ignore: avoid_print
      print("Gioi");
    } else if (grade == "B") {
      // ignore: avoid_print
      print("kha");
    } else {
      // ignore: avoid_print
      print("Trung binh");
    }

    //
    switch (grade) {
      case "A":
        // ignore: avoid_print
        print("Gioi");
        break;
      case "B":
        // ignore: avoid_print
        print("kha");
        break;
      case "C":
        break;
      default:
        // ignore: avoid_print
        print("error!");
    }

    //
    for (int i = 0; i < 5; i++) {
      // ignore: avoid_print
      print("gia tri cua i : $i");
    }

    //
    int i = 0;
    while (i < 5) {
      // ignore: avoid_print
      print(i);
      i++;
    }

//
    greet();
    greetname("DAT");
    // ignore: unused_local_variable
    int sum = add(6, 7);
    // ignore: avoid_print
    print("tong la : $sum");

    return MaterialApp(
      debugShowCheckedModeBanner: false,
      home: Scaffold(),
    );
  }
}
