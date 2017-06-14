# HW-ForeachLoops
A loop is a sequence of statements which is specified once but which may be carried out several times in succession. The code "inside" the loop (the body of the loop, shown below as xxx) is obeyed a specified number of times, or once for each of a collection of items, or until some condition is met, or indefinitely (Links to an external site.)Links to an external site..  Demonstrate concepts to the instructor and describe them in your own words. Put your work to GIT. Submit the GIT url to canvas.

public class ForeachLoop : MonoBehaviour
{
  void Start ()
  {
    string[] fruit = new string[4];
    
    fruit[0] = "Apple";
    fruit[1] = "Orange";
    fruit[2] = "Bananna";
    fruit[3] = "Pear";
    
    foreach(string item in fruit)
    {
      print (item);
    }
  }
}


Unity Example

using UnityEngine;
using System.Collections;

public class ForeachLoop : MonoBehaviour 
{   
    void Start () 
    {
        string[] strings = new string[3];
        
        strings[0] = "First string";
        strings[1] = "Second string";
        strings[2] = "Third string";
        
        foreach(string item in strings)
        {
            print (item);
        }
    }
}
