using System;
using System.Linq;
using System.Collections.Generic;

namespace HelloWorld;

class Program
{
    public static void Main()
    {

        Homepage();
    }

    // Home page

    static void Homepage()
    {
        Console.Clear();
        Console.ResetColor();
        Console.WriteLine("CP2 - ACTIVITY : OVERLOADING METHODS");
        Console.WriteLine("NAME: MICA CLAVIO");
        Console.WriteLine("CYS: ACT-1A");
        Console.WriteLine("=== BPC Preview Program ===");
        Console.WriteLine("Please  select one (enter the number only): ");

        Console.WriteLine("1. VIEW COURSES");
        Console.WriteLine("2. VIEW PROGRAMS");
        Console.WriteLine("3. VIEW CAMPUSES");
        Console.WriteLine("-------------------------");



        Console.Write("Choose an option: ");
        string choice = Console.ReadLine();

        if (choice == "1")
            Courses();
        else if (choice == "2")
            Programs();
        else if (choice == "3")
            Campuses();
        else
            Console.WriteLine("Invalid choice.");

    }

    static void Courses()
    {
        Console.ForegroundColor = ConsoleColor.Blue;
        Console.Clear();
        Console.WriteLine("VIEW COURSES\n");
        Console.WriteLine("1. Computer Programming 1");
        Console.WriteLine("2. Computer Programming 2");
        Console.WriteLine("3. Professional Ethics");
        Console.WriteLine("4. Human Computer Interaction");
        Console.WriteLine("5. Web Development");
        Console.WriteLine("6. Object Oriented Programming");
        Console.WriteLine("7. Web Applications");
        Console.WriteLine("8. Mobile Application Development");




        GoBack();

    }


    static void Programs()
    {
        Console.ForegroundColor = ConsoleColor.Red;
        Console.Clear();
        Console.WriteLine("VIEW PROGRAMS\n");

        Console.WriteLine("1. Associate in Computer Technology");
        Console.WriteLine("2. Bachelor of Science in Information Systems");
        Console.WriteLine("3. Bachelor of Science in Office Management");
        Console.WriteLine("4. Hotel and Restaurant Services");
        Console.WriteLine("5. Bachelor of Science in Custom Administration");
        Console.WriteLine("6. Contact Center Services");

        GoBack();

    }


    static void Campuses()
    {
        Console.ForegroundColor = ConsoleColor.Green;
        Console.Clear();
        Console.WriteLine("VIEW CAMPUSES\n");


        Console.WriteLine("1. MALOLOS MAIN");
        Console.WriteLine("2. SAN RAFAEL");
        Console.WriteLine("3. BOCAUE");
        Console.WriteLine("4. BUSTOS");
        Console.WriteLine("5. PANDI");
        Console.WriteLine("6. ANGAT");
        Console.WriteLine("7. MEYCAUAYAN");
        Console.WriteLine("8. SAN JOSE DEL MONTE");

        GoBack();







    }











    static void GoBack()
    {
        Console.WriteLine("Press enter to go back to Main Menu.");
        Console.ReadKey();
        Homepage();

    }






