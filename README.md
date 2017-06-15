# HW-ForeachLoops
A loop is a sequence of statements which is specified once but which may be carried out several times in succession. The code "inside" the loop (the body of the loop, shown below as xxx) is obeyed a specified number of times, or once for each of a collection of items, or until some condition is met, or indefinitely.  Demonstrate concepts to the instructor and describe them in your own words. Put your work to GIT. Submit the GIT url to canvas.

Foreach Loops go through Arrays (or Lists) and identify each string/item in it, it prints everything from the array to the Unity Console/Clear On Play, unless if the script stops/"breaks" the loop.



In this example, we see that the integer "myInt" is assigned to "fruit[2]". Then we see the amount of 4 (new) strings are created. The foreach loop will print each string, BUT, since "myInt" is the same as "fruit[2]", the loop stops.

public class ForeachLoop : MonoBehaviour
{
  
  int myInt = fruit[2];
  
  void Start ()
  {
    string[] fruit = new string[4];
    
    fruit[0] = "Apple";
    fruit[1] = "Orange";
    fruit[2] = "Bananna";
    fruit[3] = "Pear";
    
    foreach(string item in fruit)
    {
      if(myInt == fruit[2])
        break;
      
      print (item);
    }
  }
}




In this next example, this shows a different method of creating an array and strings; yet the foreach loop will work the same. It will print as "You have 3 bullet(s) left", etc.

public class Bullets : MonoBehaviour
{
  void Start()
  {
    string[] ammo = {"9", "8", "7", "6", "5", "4", "3", "2", "1", "no"};
    
    foreach(string item in ammo)
    {
      print("You have " + item + " bullet(s) left.");
    }
  }
}
