# "LV" Date Code

An intermediate level task for practicing string parsing and data conversion.

LV (multinational corporation specializing in luxury goods) handbags have "date codes" with information about a handbag manufacturing location and date. In the task you have to implement "date code" generation and parsing algorithms for different "date code" formats.

Read more about [LV's "date codes"](https://www.savvychicconsignment.com/authenticity/louis-vuitton/) before starting work on the task.

[![How to Decode a Date Code](https://www.yoogiscloset.com/media/wordpress/2019/02/how-to-read-louis-vuitton-date-code-chart.jpg)](https://www.yoogiscloset.com/blog/louis-vuitton-date-codes/)


## Get the Project

* [Open a project from your remote repository](https://docs.microsoft.com/en-us/visualstudio/get-started/tutorial-open-project-from-repo) or [get your local copy](https://docs.microsoft.com/en-us/azure/devops/repos/git/clone#clone-from-another-git-provider) with Visual Studio.


## Complete the Task

The first group of [overloaded methods](https://docs.microsoft.com/en-us/dotnet/standard/design-guidelines/member-overloading) should generate a "date code" string using a two-letter factory location code, a manufacturing year and a manufacturing month. The methods are overloaded. The one method should be implemented with "uint" parameters type, the second method should have "[DateTime](https://docs.microsoft.com/en-us/dotnet/api/system.datetime)" parameter type.

1. Implement GenerateEarly1980Code(uint, uint) and GenerateEarly1980Code(DateTime) methods in the [DateCodeGenerator.cs](LouVuiDateCode/DateCodeGenerator.cs) file.
2. Implement GenerateLate1980Code(string, uint, uint) and GenerateLate1980Code(DateTime) methods in the [DateCodeGenerator.cs](LouVuiDateCode/DateCodeGenerator.cs) file.
3. Implement Generate1990Code(string, uint, uint) and Generate1990Code(DateTime) methods in the [DateCodeGenerator.cs](LouVuiDateCode/DateCodeGenerator.cs) file.
4. Implement Generate2007Code(string, uint, uint) and Generate2007Code(DateTime) method in the [DateCodeGenerator.cs](LouVuiDateCode/DateCodeGenerator.cs) file.

Then implement a helper method that should return a list of countries that have factories with a specified factory location code. Two or more countries may have factories with the same location code (ex. France and USA have a factory with "SD" location code). Countries are implemented as [enumeration type values](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/enum).

5. Implement GetCountry method in the [CountryParser.cs](LouVuiDateCode/CountryParser.cs) file.

The next group of methods should parse a "date code" string and return the manufacturing data in [out parameters](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/out-parameter-modifier).

6. Implement ParseEarly1980Code method in the [DateCodeParser.cs](LouVuiDateCode/DateCodeParser.cs) file.
7. Implement ParseLate1980Code method in the [DateCodeParser.cs](LouVuiDateCode/DateCodeParser.cs) file.
8. Implement Parse1990Code method in the [DateCodeParser.cs](LouVuiDateCode/DateCodeParser.cs) file.
9. Implement Parse2007Code method in the [DateCodeParser.cs](LouVuiDateCode/DateCodeParser.cs) file.

Check out "See also" section for the methods and classes you may use to solve the task.


## Fix Compiler Issues

Additional style and code checks are enabled for the projects in this solution to help you maintaining consistency of the project source code and avoiding silly mistakes. [Review the Error List](https://docs.microsoft.com/en-us/visualstudio/ide/find-and-fix-code-errors#review-the-error-list) in Visual Studio to see all compiler warnings and errors.

If a compiler error or warning message is not clear, [review errors details](https://docs.microsoft.com/en-us/visualstudio/ide/find-and-fix-code-errors#review-errors-in-detail) or google the error or warning code to get more information about the issue.


## Save Your Work

* [Rebuild your solution](https://docs.microsoft.com/en-us/visualstudio/ide/building-and-cleaning-projects-and-solutions-in-visual-studio) in Visual Studio.
* Check out the [Error List window](https://docs.microsoft.com/en-us/visualstudio/ide/reference/error-list-window) for compiler errors and warnings. If you have any of those issues, **fix issues** and rebuild the solution again.
* [Run all unit tests with Test Explorer](https://docs.microsoft.com/en-us/visualstudio/test/run-unit-tests-with-test-explorer) and make sure there are **no failed unit tests**. Fix your code to [make all your unit tests GREEN](https://stackoverflow.com/questions/276813/what-is-red-green-testing).
* Review all your changes **before** saving your work.
    * Open "Changes" view in [Team Explorer](https://docs.microsoft.com/en-us/visualstudio/ide/reference/team-explorer-reference).
    * Click with your right mouse button on a modified file.
    * Click on "Compare with Unmodified" menu item to open a comparison window.
* [Stage your changes](https://docs.microsoft.com/en-us/azure/devops/repos/git/commits#stage-your-changes) and [create a commit](https://docs.microsoft.com/en-us/azure/devops/repos/git/commits#create-a-commit).
* Share your changes by [pushing them to remote repository](https://docs.microsoft.com/en-us/azure/devops/repos/git/pushing).


## See also

* Tutorials
  * [Indices and ranges](https://docs.microsoft.com/en-us/dotnet/csharp/tutorials/ranges-indexes)
* .NET Guide
  * [Standard numeric format strings](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-numeric-format-strings)
  * [How to: Pad a Number with Leading Zeros](https://docs.microsoft.com/en-us/dotnet/standard/base-types/how-to-pad-a-number-with-leading-zeros)
* C# Reference
  * [Enumeration types](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/enum)
  * [out parameter modifier](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/out-parameter-modifier)
* .NET API
  * [String.Length Property](https://docs.microsoft.com/en-us/dotnet/api/system.string.length)
  * [String.Chars Property](https://docs.microsoft.com/en-us/dotnet/api/system.string.chars)
  * [String.Format Method](https://docs.microsoft.com/en-us/dotnet/api/system.string.format)
  * [String.ToUpper Method](https://docs.microsoft.com/en-us/dotnet/api/system.string.toupper)
  * [UInt32.ToString Method](https://docs.microsoft.com/en-us/dotnet/api/system.uint32.tostring)
  * [Char.IsLetter Method](https://docs.microsoft.com/en-us/dotnet/api/system.char.isletter)
  * [Array.IndexOf Method](https://docs.microsoft.com/en-us/dotnet/api/system.array.indexof)
  * [Enum Class](https://docs.microsoft.com/en-us/dotnet/api/system.enum)
  * [CultureInfo Class](https://docs.microsoft.com/en-us/dotnet/api/system.globalization.cultureinfo)
  * [GregorianCalendar Class](https://docs.microsoft.com/en-us/dotnet/api/system.globalization.gregoriancalendar)
  * [DateTime Struct](https://docs.microsoft.com/en-us/dotnet/api/system.datetime)
