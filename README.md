# HW-Lists
Watch read and practice from the module: Arrays and Lists  Write your understanding of the topic using comments and examples (at least 10 examples) to the instructor and describe them in your own words to the best of your knowledge. Put your work to GIT. Submit the GIT url to canvas. 

#1

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

#2

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

#5

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
  }
}

#6

public static void Main()
{
 List<string> gameConsoles = new List<string>();
  
 gameConsoles.Add("PlayStation");
 gameConsoles.Add("Nintendo");
 gameConsoles.Add("Xbox");
 
 gameConsoles.Remove("Xbox");
 print(gameConsoles.Count);
}

#7

public static void Main()
{
 List<string> gameConsoles = new List<string>();
  
 gameConsoles.Add("PlayStation");
 gameConsoles.Add("Nintendo");
 gameConsoles.Add("Xbox");
 
 gameConsoles.RemoveAt(3);
 print(gameConsoles.Count);
}

#8

public static void Main()
{
  List<string> clothes = new List<string>();
  
  clothes.Add("shirt");
  clothes.Add("pants");
  clothes.Add("shoes");
  
  clothes.Remove("pants");
  print(clothes.Count);
}

#9

public static void Main()
{
  List<string> clothes = new List<string>();
  
  clothes.Add("shirt");
  clothes.Add("pants");
  clothes.Add("shoes");
  
  clothes.RemoveAt("2");
  print(clothes.Count);
}

#10

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
