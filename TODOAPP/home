import 'package:confirm_dialog/confirm_dialog.dart';
import 'package:flutter/material.dart';
import 'package:flutter_application_1/page/dialog_box.dart';
import 'package:flutter_application_1/page/todolist.dart';

// ignore: must_be_immutable
class Homepage extends StatefulWidget {
  const Homepage({super.key});

  @override
  State<Homepage> createState() => _HomepageState();
}

TextEditingController controller = TextEditingController();

class _HomepageState extends State<Homepage> {
  List job = [];

  void onchangedcheckbox(int index, bool? value) {
    setState(() {
      job[index][1] = value;
    });
  }

  void onsave() {
    setState(() {
      job.add([controller.text, false]);
      Navigator.of(context).pop();
    });
    controller.clear();
  }

  void createnewtask() {
    showDialog(
      context: context,
      builder: (context) {
        return DialogBox(
          controller: controller,
          onsave: () => onsave(),
          oncansel: () => Navigator.of(context).pop(),
        );
      },
    );
  }

  void deletask(int index) {
    setState(() {
      job.removeAt(index);
    });
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: const Color.fromARGB(255, 227, 195, 97),
      appBar: AppBar(
        backgroundColor: Colors.blueAccent,
        title: Center(
          child: Text("TO DO APP"),
        ),
      ),
      floatingActionButton: FloatingActionButton(
        onPressed: createnewtask,
        // ignore: sort_child_properties_last
        child: Icon(Icons.add),
        backgroundColor: Colors.blue,
      ),
      body: ListView.builder(
        itemCount: job.length,
        itemBuilder: (context, index) => Todolist(
          taskname: job[index][0],
          selected: job[index][1],
          onchanged: (value) => onchangedcheckbox(index, value),
          deletask: () async {
            if (await confirm(context)) {
              // ignore: avoid_print
              return deletask(index);
            }
            // ignore: avoid_print
            return;
          },
        ),
      ),
    );
  }
}
