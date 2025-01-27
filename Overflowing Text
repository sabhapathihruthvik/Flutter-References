import 'package:flutter/material.dart';

void main() {
  runApp(const OverflowTextDemo());
}

class OverflowTextDemo extends StatelessWidget {
  const OverflowTextDemo({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: const Text("Overflow Text Demo"),
        ),
        body: Padding(
          padding: const EdgeInsets.all(16.0),
          child: SingleChildScrollView(
            child: Column(
              crossAxisAlignment: CrossAxisAlignment.start,
              children: [
                const Text(
                  "1. TextOverflow.ellipsis (Single Line):",
                  style: TextStyle(fontSize: 16, fontWeight: FontWeight.bold),
                ),
                Container(
                  color: Colors.blue[50],
                  child: const Text(
                    "This is a very long text that should overflow and display with ellipsis...",
                    overflow: TextOverflow.ellipsis,
                    maxLines: 1,
                  ),
                ),
                const SizedBox(height: 16),
                const Text(
                  "2. TextOverflow.clip (Single Line):",
                  style: TextStyle(fontSize: 16, fontWeight: FontWeight.bold),
                ),
                Container(
                  color: Colors.green[50],
                  child: const Text(
                    "This is a very long text that will overflow but be clipped overflowingoverflowing.",
                    overflow: TextOverflow.clip,
                    maxLines: 1,
                  ),
                ),
                const SizedBox(height: 16),
                const Text(
                  "3. TextOverflow.fade (Single Line):",
                  style: TextStyle(fontSize: 16, fontWeight: FontWeight.bold),
                ),
                Container(
                  color: Colors.orange[50],
                  child: const Text(
                    "This is a very long text that will fade when overflowing overflowing overflowing.",
                    overflow: TextOverflow.fade,
                    maxLines: 1,
                  ),
                ),
                const SizedBox(height: 16),
                const Text(
                  "4. Multi-line with maxLines:",
                  style: TextStyle(fontSize: 16, fontWeight: FontWeight.bold),
                ),
                Container(
                  color: Colors.purple[50],
                  child: const Text(
                    "This is a multi-line text that demonstrates maxLines property. It will display only up to 2 lines and truncate the rest with ellipsis if needed.",
                    maxLines: 2,
                    overflow: TextOverflow.ellipsis,
                  ),
                ),
                const SizedBox(height: 16),
                const Text(
                  "5. Wrapping Text in a Wrap Widget:",
                  style: TextStyle(fontSize: 16, fontWeight: FontWeight.bold),
                ),
                Container(
                  color: Colors.red[50],
                  child: const Wrap(
                    children: [
                      Text(
                        "This is text inside a Wrap widget. It will wrap and never overflow since it dynamically adjusts to the available width.",
                      ),
                    ],
                  ),
                ),
                const SizedBox(height: 16),
                const Text(
                  "6. Scrolling Text:",
                  style: TextStyle(fontSize: 16, fontWeight: FontWeight.bold),
                ),
                Container(
                  height: 100,
                  color: Colors.teal[50],
                  child: const SingleChildScrollView(
                    child: Text(
                      "This is a long text that exceeds the container's height. You can scroll through it to see the full content.This is a long text that exceeds the container's height. You can scroll through it to see the full content.This is a long text that exceeds the container's height. You can scroll through it to see the full content.",
                    ),
                  ),
                ),
                const SizedBox(height: 16),
                const Text(
                  "7. Flexible Widget (in Row):",
                  style: TextStyle(fontSize: 16, fontWeight: FontWeight.bold),
                ),
                const Row(
                  children: [
                    Icon(Icons.text_fields),
                    Flexible(
                      child: Text(
                        "This is a long text inside a Row that uses Flexible to prevent overflow.",
                        overflow: TextOverflow.ellipsis,
                      ),
                    ),
                  ],
                ),
                const SizedBox(height: 16),
                const Text(
                  "8. FittedBox:",
                  style: TextStyle(fontSize: 16, fontWeight: FontWeight.bold),
                ),
                Container(
                  color: Colors.yellow[50],
                  child: const FittedBox(
                    child: Text(
                      "This text will scale to fit within the container using .",
                    ),
                  ),
                ),
              ],
            ),
          ),
        ),
      ),
    );
  }
}
