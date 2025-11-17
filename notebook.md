# My coding Notebook

## Table of Contents
- [Flutter notes](#flutter-notes)
  - [What is flutter](#what-is-flutter)
  - [key terms and definitions](#key-terms-and-definitions)
  - [layout and design widgets](#layout-and-design-widgets)
  - [Flutter Definitions with Structures](#flutter-definitions-with-struture)
- [Code Definitions](#code-definitions)
- [notebook Style Guide](#markdown-style-guide-for-coding-notebooks)


## Flutter Notes

### What is Flutter?
- Definition:a framework made by Google for building apps that work on web, Android, and IOS - with one codebase.
- Why is it useful? It lets us make it for all bases with one code so we don't have to do it multiple times for the different bases.

---

### Key Terms and Definitions

| Term             | Definition                                      | Example / Notes                          |
|------------------|--------------------------------------------------|-------------------------------------------|
| Widget           | basic building block of a flutter app. Everything is a Widget.                           | Text, Image, Container, Column                                          |
| MaterialApp      | The root of the app. Sets up routes and themes                                                | Found in mainn.dart                                          |
| Scaffold         | probides basic visual layout- like a header, body, floating buttom                                                 | EACH SCREEN USES IT                                          |
| StatelessWidget  |a widget that doiesn't change                                               |  most of the screen files                                        |
| StatefulWidget   | a widget that can change over time                                                | Used in MyHomePage()                                          |
| Navigator        | manages screen transitions                                                 | Navigator.pushNamed(context, '/page2'):                                          |
| AppBar           | Top navigation bar                                                 | Title of each page appears here                                           |
| Column           |  vertical layout                                 |                                           |
| Row              |  horizontal layout                               |                                           |
| Container        |  wraps content with padding, margin, or color    |                                           |
| Text             |  displays text                                   |                                           |
| Image.network    |  displays images from a URL                      |                                           |
| Padding          |  adds space around a widget                      |                                           |
| Center |            centers its child                               |                                           |
| named routes| predefinded paths to navigate between scrrens | '/', '/page2', '/page3',ect   |
|main()| The funtion thqt runs the app|found in main.dart|
---




### Layout and Design Widgets
- How do you center a widget?
- How do you align something to the left or right?
- What widget adds space around content?

<img width="1201" height="400" alt="image" src="https://github.com/user-attachments/assets/48d37a85-576d-42d5-a99f-843eef7fa28a" />



Follow this guide to keep your coding notebook **clear, consistent, and professional**.  
This ensures your notes are easy for you (and others) to read later.

---

## 🔹 Headings
**When to use:** Organize your notebook into sections (like days, topics, or projects).  
- `#` for the notebook title (use once at the top).  
- `##` for each day or major topic.  
- `###` for subsections (like "Notes", "Practice", "Reflections").  

✅ Example:


# My Coding Notebook
## Day 1
### Notes
### Practice

🔡 Text Formatting
When to use: Highlight important ideas or add emphasis.

Use bold for key terms or definitions.

Use italic for emphasis or side comments.

Use inline code for keywords, functions, or commands.

 

✅ Example:

**Class** = a blueprint for objects  
*Remember:* always test your code  
Use `System.out.println()` to print

 

💻 Code Blocks
When to use: Anytime you write multiple lines of code.

Inline code for short snippets.

Fenced code blocks with language for full examples.

✅ Example:

```java
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

🧾 Lists
When to use: Organize steps, notes, or key points.

Numbered lists for sequences or steps.

Bulleted lists for unordered ideas.

✅ Example:

1. Define the class
2. Write the main method
3. Test your program

Variables
- Loops
- Conditionals
 

✅ Checklists
When to use: Track progress on assignments or tasks.

✅ Example:

[x] Complete coding warm-up
- [ ] Finish project draft
- [ ] Reflect on learning

 

➡️ Blockquotes
When to use: Call out notes, reminders, or teacher comments.

✅ Example:

> 💡 Remember: Loops repeat code until a condition is false.

 

📊 Tables
When to use: Compare values, track progress, or organize data neatly.

✅ Example:

| Task        | Status   | Notes          |
|-------------|----------|----------------|
| Homework 1  | Done ✅  | Submitted      |
| Homework 2  | Pending  | Needs review   |

 

🔗 Links & Images
When to use: Add references, resources, or visuals.

✅ Example:

[Java Docs](https://docs.oracle.com/javase/8/docs/api/)  
![Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)

 

📂 Collapsible Sections
When to use: Hide solutions, extended notes, or extra details.

✅ Example:

<details>
  <summary>Click to reveal solution</summary>
  
System.out.println("Answer: 42");

</details>

 

📝 Footnotes
When to use: Add references or side notes without cluttering the page.

✅ Example:

This concept is related to object-oriented programming.[^1]

[^1]: See "Objects and Classes" in your textbook.

 

🎯 Style Rules
Consistency matters more than creativity

Always use headings to structure your notes.

Always use code blocks for multi-line code.

Clarity first

Bold key terms.

Use lists instead of long sentences when outlining steps.

Professional tone

Don’t mix casual notes with formal work in the same section.

Use blockquotes for reflections or teacher feedback.

Track your learning

Use checklists to mark what’s done.

Use collapsible sections if you want to hide answers until review time.

 

✅ Bottom Line:

Headings = Structure

Bold/Italic = Emphasis

Code blocks = Code

Lists = Steps/Ideas

Tables = Organization

Checklists = Progress

Blockquotes = Notes/Tips

Collapsible = Hide/Show detail

Keep it simple, consistent, and clear.

## Flutter Definitions With Structures
| Term | Definition and Description | Base Structure | Real Life Example | App Example |
|------|----------------------------|----------------|-------------------|-------------|
|   main   | A function that runs when your app starts. It tells Flutter what app to show. | `void main() => runApp(MyApp());` | a car starting | void main() => runApp(MyPortfolioApp());  |
|   MaterialApp   | The widget that sets up your whole app’s look and navigation. | `MaterialApp(...)` |  | eturn MaterialApp(debugShowCheckedModeBanner: false,title: 'TSA Portfolio',theme: ThemeData( and more |
|   Scaffold   | A widget that gives you the basic layout: background, navigation bar, floating button, etc. | `Scaffold(...)` | any template | return Scaffold(body: Column(mainAxisAlignment: MainAxisAlignment.start,children: [ and more|
|   Column   | A widget that holds and displays your content in a straight line from top to bottom. | `Column(...)` |  |  Column(children: [const Padding(padding: EdgeInsets.all(8.0),child: Text.rich( and more|
|    Row  | A widget that shows things side-by-side. | `Row(...)` |  | Row(children: [ClipRRect( borderRadius: BorderRadius.circular(8), and more|
|    Container  | A box that holds other widgets. You can add color, padding, borders, or size. | `Container(...)` |  |  return Container(margin: const EdgeInsets.symmetric(vertical: 8, horizontal: 16),padding: const EdgeInsets.all(12),decoration: BoxDecoration(border: Border.all(color: Colors.blue),borderRadius: BorderRadius.circular(12),), child: Row(and more|
|   Text   | A widget to display text on the screen. | `Text('Hello')` |  | child: Text(description,style: const TextStyle(color: Colors.white),), |
|   image.network  | A widget to show an image using a link from the internet. | `Image.network('https://...')` |  | "image": "https://placedog.net/550", |
|   Elevatedbutton   | A clickable button that floats above content. You choose what happens when it's clicked. | `ElevatedButton(onPressed: ..., child: ...)` |  |  |
|    onPressed  | The code that gets run when a button is tapped or something happens. | `onPressed: () => doSomething()` |  |  |
|   Stateless Widget   | A class that creates widgets that never change. Good for static screens. | `class HomeScreen extends StatelessWidget` |  |  |
|   Statefull Widget   | A class for widgets that can change while the app is running. | `class MyWidget extends StatefulWidget` |  |  |
|   Navigator   | Lets you move from one screen to another using route names. | `Navigator.pushNamed(context, '/about')` |  |  |
|   padding   | Makes space around a widget inside its container. | `Padding(padding: EdgeInsets.all(8.0), child: ...)` |  |  
|   center   | Aligns content in the center of the screen or container. | `Center(child: ...)` |  |  |
|   wrap   | Automatically puts widgets onto a new line when there's no space. | `Wrap(children: [...])` |  |  |
|   @override   | This marks a method as one that’s replacing a method in a parent class. | `@override` |  | @overrideWidget build(BuildContext context) {final List<Map<String, String>> dogInfo = [ |
|   Build widget   | The special function in every widget that describes what gets drawn on the screen. | `Widget build(BuildContext context) {...}` |  |  |
|   Build   | Required in every widget class to describe what to show. | `build` |  |  |
|   Build Context   | A variable that helps the widget know where it is and lets it communicate with the app. | `BuildContext context` |  |  |
|   super.key   | A keyword used to pass a value to the parent widget. | `super.key` |  | const MyPortfolioApp({super.key}); |
|   const   | A keyword that means the value won't change and is set once. | `const` |  |  |


## Code Definitions
| Term | Definition | Base Structure / Syntax | Real Life Example | App Example |
|------|------------|--------------------------|-------------------|-------------|
| Algorithms | Define step by step processes to follow when completing a task or solving a problem | no syntax | Make a grilled cheese | Verify user |
| Sequencing | Define an order for when steps in an algorithm are completed | Follows 1, 2, 3 | which step comes first in making a grilled cheese | Get bread, add butter, add cheese |
|   Variable   | A named container used to store a value that may change. | `var x = 5;` |  Goals in soccer| main.dart, string title:  title: 'TSA Portfolio' |
|   Constant   | A fixed value that cannot change once set. | `const PI = 3.14;` | your Username | const MyPortfolioApp({super.key}); |
|   Data Type   | The kind of value a variable holds, like numbers or text. | `int`, `String`, `bool` | Videos or numbers |  |
|   String   | A sequence of characters used to represent words or text. | `"Hello World"` | words  | Titles on a website|
|  Integer    | Whole number values. | `int age = 16;` | days on a calender | the total number of notifications you have |
|   Double   | Number values with decimals. | `double age = 16.2;` |  | animations |
|   Boolean   | A value that can be true or false. | `bool isLoggedIn = false;` | are the lights on or not |  |
|   List   | A collection of values in a specific order. | `List<String> names = [];` | A wallet or a grocery list |  |
|   Null   | A special value that means “nothing.” | `String? name = null;` |   |  |
|   Funtion   | A reusable block of code that performs an action. | `void sayHi() { print("Hi"); }` |  |  |
|   Parameter   | The information passed into a function to change how it works. | `greet(String name)` | information that can change |  |
|   return   | The result a function gives back. | `return total;` |  |  |
|   Scope   | Where a variable or function can be used. | (No set syntax — concept-based) | a class in school |  |
|   Class   | Blueprint for creating objects with specific structure and behavior. | `class Dog {}` |  |  |
|   Object   | A specific version of a class. | `Dog myDog = Dog();` |  |  |
|    property  | A variable that belongs to a class/object. | `String name;` |  |  |
|   Method   | A function that belongs to a class. | `void bark() {}` |  |  |
|    constructor  | A special function used to set up a class when it’s created. | `Dog(this.name);` |  |  |
|   Abstraction   | Hiding the inner workings of code so users only interact with what they need. | (Concept — not specific code) |  |  |
|   Override   | Changing how a built-in or inherited function behaves. | `@override` | most stats being the same but one person might have better stats |  |
|   Void   | A function that does not return a value. | `void printMessage() {}` |  |  |



