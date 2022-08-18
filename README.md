# CMPG 323 Project Overview
<img src="https://github.com/ChiefMonk/CMPG-323-Overview-37016776/blob/main/nwu_logo.jpg" width="100" /> 

The overview document explains the overall project structure for the semester, and the general branching strategy for each project repository and also serves as a general guide to everything about this semester's projects for CMPG 323.

## Project Structure
For the work to be done this semester, a single <a href="https://github.com/users/ChiefMonk/projects/5">Kanban project</a> is created to outline and plan for all the work to be done. The scheduled work will be done over 8 Sprints, each lasting 10 working days (2 calendar weeks). At the beginning of every sprint, mostly on the first day, a sprint planning session is convened to categorise and itemise what will be done and allocate appropriate resources and time to each issue. 

However, to properly manage the project and meet the various sprint deadlines, the work is further planned and divided weekly. This also helps to negate any time challenges that could be encountered over the 2-week fixed time period.
 

Now, let us perform Bubble Sort.

Start with the first two elements 78 and 55. 55 is smaller than 78, so swap both of them. Now the list is −
```
55, 78,45,98, 13
```

Now 45 is less than 78, so swap it.
```
55, 45, 78, 98, 3
```

Now 98 is greater than 78, so keep as it is.
3 is less than 98, so swap it. Now the list looks like −
```
55, 45, 78, 3, 98
```

This was the first iteration. After performing all the iterations, e will get our sorted array using Bubble Sort −
```
3, 45, 55, 78, 93
```

## Code Example
Let us see an example with X elements in an array and sort it.
```
using System;

namespace CMPG323._37016776.BubbleSort
{
	internal class Program
	{
		static void Main(string[] args)
		{
			Console.WriteLine("CMPG 323 Homework Exercise 1 & 2: Bubble Sort Algorithm using C");
			Console.WriteLine();

			int arraySize = 0;

			while (arraySize < 2)
			{
				try
				{
					Console.Write("How many integers go you want to sort:  ");
					arraySize = int.Parse(Console.ReadLine() ?? string.Empty);
				}
				catch
				{
					Console.WriteLine("Please enter a valid integer greater than 2");
					Console.WriteLine();
				}
			}

			Console.WriteLine();
			Console.WriteLine($"Please enter the {arraySize} integers to be sorted, one at a time");
			int[] inputArray = new int[arraySize];
			int counter = 0;

			while (counter < arraySize)
			{
				try
				{
					Console.Write($"Enter integer {counter + 1}: ");
					inputArray[counter] = int.Parse(Console.ReadLine() ?? string.Empty);
					counter++;
				}
				catch
				{
					Console.WriteLine("Please enter a valid integer");
					Console.WriteLine();
				}
			}

			BubbleSortArray(inputArray);
			Console.WriteLine();
			Console.Write("Sorted Array: [ ");
			foreach (var p in inputArray)
				Console.Write(p + " ");
			Console.Write("]");
			Console.WriteLine();
			Console.WriteLine();
			Console.WriteLine("Press ENTER to Exit the program");
			Console.Read();
		}

		private static void BubbleSortArray(int[] inputArray)
		{
			for (int j = 0; j <= inputArray.Length - 2; j++)
			{
				for (int i = 0; i <= inputArray.Length - 2; i++)
				{
					if (inputArray[i] > inputArray[i + 1])
					{
						var temp = inputArray[i + 1];
						inputArray[i + 1] = inputArray[i];
						inputArray[i] = temp;
					}
				}
			}
		}
	}
}
```

## Output
Sorted Array:
```
[ 13 45 55 78 98 ]
```

## Links
### Source Control – Git (with GitHub)
* [Introduction to version control with Git](https://docs.microsoft.com/en-us/learn/paths/intro-to-vc-git/)
* [Visual Studio version control docs](https://docs.microsoft.com/en-us/visualstudio/version-control/?wt.mc_id=learnredirect_githubvscode_content_cnl_csaapp&view=vs-2022)
* [Build community-driven software projects on GitHub](https://docs.microsoft.com/en-gb/learn/paths/build-community-driven-projects-github/)
### Azure Fundamentals
* [Microsoft Certified: Azure Fundamentals](https://docs.microsoft.com/en-us/certifications/azure-fundamentals/)

## Contributors
* [Chipo Hamayobe](https://github.com/ChiefMonk) - Project Lead

