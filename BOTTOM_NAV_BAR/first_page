import 'package:flutter/material.dart';
import 'package:flutter_application_1/page/home_page.dart';
import 'package:flutter_application_1/page/profile_page.dart';
import 'package:flutter_application_1/page/setting_page.dart';

// ignore: must_be_immutable
class FirstPage extends StatefulWidget {
  const FirstPage({super.key});

  @override
  State<FirstPage> createState() => _FirstPageState();
}

class _FirstPageState extends State<FirstPage> {
  //method updated selectedindex
  void navigatebottombar(int index) {
    setState(() {
      selectedindex = index;
    });
  }

  int selectedindex = 0;

  final List page = [
    HomePage(),
    ProfilePage(),
    SettingPage(),
  ];

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        backgroundColor: Colors.deepPurpleAccent,
        title: Center(
          child: Text("My App"),
        ),
      ),
      body: page[selectedindex],
      bottomNavigationBar: BottomNavigationBar(
        //onTap: navigatebottombar,
        onTap: (index) {
          navigatebottombar(index);
        },
        currentIndex: selectedindex,
        items: [
          //Home
          BottomNavigationBarItem(
            icon: Icon(Icons.home),
            label: "Home",
          ),

          //Profile

          BottomNavigationBarItem(
            icon: Icon(Icons.person),
            label: "profile",
          ),

          //Setting

          BottomNavigationBarItem(
            icon: Icon(Icons.settings),
            label: "Sittings",
          ),
        ],
      ),
    );
  }
}
