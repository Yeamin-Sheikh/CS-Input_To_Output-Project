# CS-Input_To_Output-Project
A repository containing basic CS code that Takes input and outputs the result.

<br/>

## Main Code  
```
using System;

namespace input_To_Output
{
    internal class Program
    {
        static void Main(string[] args)
        {
            try 
	        {
                Console.WriteLine("---ENTER INFO---");
                Console.Write("Institution Name: ");
                string iName = Console.ReadLine();
                Console.Write("Student Name: ");
                string sName = Console.ReadLine();
                Console.Write("Department: ");
                string dep = Console.ReadLine();
                Console.Write("Roll: ");
                int roll = Convert.ToInt32(Console.ReadLine());

                Console.WriteLine("\n---FULL INFORMATION--- \nInstitution Name: {0} \nStudent Name: {1} \nDepartment: {2} \nRoll: {3}", iName, sName, dep, roll);
            }
	        catch (FormatException e)
	        {
                Console.WriteLine(e.Message);
            }
            catch (Exception e)
	        {
                Console.WriteLine("Something Went Wrong! Restart the program.");
            }
            finally
            {
                Console.WriteLine("Press any key to exit.");
                Console.ReadKey();
            }
        }
    }
}
```
