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



#6



#7



#8



#9



#10



