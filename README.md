# HW-Lists
Watch read and practice from the module: Arrays and Lists  Write your understanding of the topic using comments and examples (at least 10 examples) to the instructor and describe them in your own words to the best of your knowledge. Put your work to GIT. Submit the GIT url to canvas.

//The first 4 examples are from today's class. 2, 3, & 4 produce the same result, but each with different operators.

#1

//By doing this example in a script, (according to the Unity Inspector) the "Size" is already sey to zero (no elements are listed). But if you type 3 into Size, the names - Jenny, Bill, & Bob, - will already appear in the newly shown elements (element 0 - Jenny, etc.). type 4 or a higher number in, then more empty elements be created, and new names to can be included. The best part is that you can perform this in Unity while it is currently in RunTime or Play Mode.

public class ArraryAndLists : MonoBehaviour
{
  public List<string> players = new List<string>();

  void Start ()
  {
    players.Add("Jenny");
    players.Add("Bill");
    players.Add("Bob");
  }
}


//2, 3, 4 - After creating the InputField & Button, you can type in more names into the "InputField", once you're done, you can click on the "Button", and information will come up on the Console/Clear on Play. This can (also) work while Unity is in Play Mode.

#2

//The purpose of using "!=", and "player*s*" first (in the if statement), is so that the code can be fast enough that it doesn't have to run.

public class ArraryAndLists : MonoBehaviour
{
  public List<string> players = new List<string>();

  public void ClickHere (string _s)
  {
  players.Add(_s);
  }

  public void RunLoop ()
  {
    foreach (string item in players)
    {
      print(item);
    }
    if (players.Count != 1)
    {
      print("You have " + players.Count + " players.");
    }
    else
    {
      print("You have " + players.Count + " player.");
    }
  }
}

#3

//Using &&, anything more than 2 or less than zero, will result in one player.

public class ArraryAndLists : MonoBehaviour
{
  public List<string> players = new List<string>();

  public void ClickHere (string _s)
  {
  players.Add(_s);
  }

  public void RunLoop ()
  {
    foreach (string item in players)
    {
      print(item);
    }
    if (players.Count > 2 && players.Count < 0)
    {
      print("You have " + players.Count + " player.");
    }
    else
    {
      print("You have " + players.Count + " players.");
    }
  }
}

#4

//Using "==", if the number you input is 1, it will say that you only have one player.

public class ArraryAndLists : MonoBehaviour
{
  public List<string> players = new List<string>();

  public void ClickHere (string _s)
  {
  players.Add(_s);
  }

  public void RunLoop ()
  {
    foreach (string item in players)
    {
      print(item);
    }
    if (players.Count == 1)
    {
      print("You have " + players.Count + " player.");
    }
    else
    {
      print("You have " + players.Count + " players.");
    }
  }
}


//The next one is based on a Unity Tutorial.

#5

//Making a list is one way to specify your class/classes.

using UnityEngine;
using System.Collections;
using System.Collections.Generic

public class FruitClass : MonoBehaviour
{
  void Start ()
  {
    List<string> fruit = new List<string>();
    
    fruit.Add("Apple");
    fruit.Add("Pear");
    fruit.Add("Orange");
    
    print("I bought " + fruit.Count + " pieces of fruit.")
  }
}


//The next four are based on the examples from http://learncs.org/en/Lists

#6

//The .Remove parameter can exclude a specific item in a list.

public static void Main()
{
 List<string> gameConsoles = new List<string>();
  
 gameConsoles.Add("PlayStation");
 gameConsoles.Add("Nintendo");
 gameConsoles.Add("Xbox");
 
 gameConsoles.Remove("Xbox");
 print(gameConsoles.Count);
}

OUTPUT: 2

#7

//The .RemoveAt parameter can take off an item's index from the list. "Xbox" is the third index.

public static void Main()
{
 List<string> gameConsoles = new List<string>();
  
 gameConsoles.Add("PlayStation");
 gameConsoles.Add("Nintendo");
 gameConsoles.Add("Xbox");
 
 gameConsoles.RemoveAt(3);
 print(gameConsoles.Count);
}

OUTPUT: 2

#8

//Similar to #6 (only its "no shirt, no shoes, no service").

public static void Main()
{
  List<string> clothes = new List<string>();
  
  clothes.Add("shirt");
  clothes.Add("pants");
  clothes.Add("shoes");
  
  clothes.Remove("pants");
  print(clothes.Count);
}

OUTPUT: 2

#9

//Similar to #7.

public static void Main()
{
  List<string> clothes = new List<string>();
  
  clothes.Add("shirt");
  clothes.Add("pants");
  clothes.Add("shoes");
  
  clothes.RemoveAt("2");
  print(clothes.Count);
}

OUTPUT: 2

#10

//In this example, you can add up the total amount of items from each list together.

public static void Main()
{
  List<string> tool = new List<string>();
  tool.Add("Hammer");
  tool.Add("Wrench");
  
  List<string> machine = new List<string>();
  machine.Add("Car");
  machine.Add ("Robot");
  
  tool.AddRange(machine);
  print(tool.Count);
}

OUTPUT: 4
