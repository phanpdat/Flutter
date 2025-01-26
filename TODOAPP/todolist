import 'package:flutter/material.dart';

class Todolist extends StatelessWidget {
  final String taskname;
  final bool selected;
  final Function(bool?)? onchanged;
  final Function()? deletask;
  const Todolist({
    super.key,
    required this.taskname,
    required this.selected,
    required this.onchanged,
    required this.deletask,
  });

  @override
  Widget build(BuildContext context) {
    return Padding(
      padding: const EdgeInsets.all(20),
      child: Container(
        // ignore: sort_child_properties_last
        child: Row(
          mainAxisAlignment: MainAxisAlignment.spaceBetween,
          children: [
            Row(
              children: [
                Checkbox(value: selected, onChanged: onchanged),
                Text(
                  taskname,
                  style: TextStyle(
                    decoration: selected
                        ? TextDecoration.lineThrough
                        : TextDecoration.none,
                  ),
                ),
              ],
            ),
            IconButton(onPressed: deletask, icon: Icon(Icons.delete))
          ],
        ),
        padding: EdgeInsets.all(15),
        decoration: BoxDecoration(
          borderRadius: BorderRadius.circular(20),
          color: Colors.amberAccent,
        ),
      ),
    );
  }
}
