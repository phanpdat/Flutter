import 'package:flutter/material.dart';

// ignore: must_be_immutable
class DialogBox extends StatelessWidget {
  DialogBox({
    super.key,
    required this.controller,
    required this.onsave,
    required this.oncansel,
  });

  VoidCallback onsave;
  VoidCallback oncansel;
  // ignore: prefer_typing_uninitialized_variables
  final controller;
  @override
  Widget build(BuildContext context) {
    return AlertDialog(
      backgroundColor: Colors.blue,
      title: Column(
        children: [
          Text("Take your job"),
          Padding(
            padding: const EdgeInsets.only(bottom: 20, top: 20),
            child: TextField(
              controller: controller,
              decoration: InputDecoration(
                  border: OutlineInputBorder(),
                  // hintText: "Mời Nhập ...",
                  label: Text("Mời Nhập ... ")),
            ),
          ),
          Row(
            mainAxisAlignment: MainAxisAlignment.end,
            children: [
              ElevatedButton(
                onPressed: oncansel,
                child: Text("Cansel"),
              ),
              Padding(
                padding: const EdgeInsets.only(left: 10),
                child: ElevatedButton(
                  onPressed: onsave,
                  child: Text("Save"),
                ),
              ),
            ],
          ),
        ],
      ),
    );
  }
}
