C# (C Sharp)
=====================================

## Goals

- Take the course from [Microsoft Virtual Academy](https://mva.microsoft.com/) to learn .Net Core and check if MVA covers everything for people who are going to develop using C# or not.
If not, then write down which part it doesn't cover.
- Also, check another websites to learn C# and compare which one is better.

What is C# ?
-------------------------------------

C# (programming language) is multi-paradigm programming language encompassing strong typing, imperative, declarative, functional, generic, object-oriented (class-based), and component-oriented programming disciplines. It was developed by Microsoft within its .  
Reference [C Sharp (programming language)](https://en.wikipedia.org/wiki/C_Sharp_(programming_language))


## [C# Fundamentals for Absolute Beginners](https://mva.microsoft.com/en-US/training-courses/c-fundamentals-for-absolute-beginners-16169?l=l5iWxYQIC_1306218949)
This introduction of C# is provided on MVA.
This video is really good for people who just start learning C#.
However, what the issue in this video is this video explain some stuff so fast and briefly somtimes.(e.g. using, System, and namespace)
To oversome it, I recommend this documentation below  
[Getting Started with C#](https://www.microsoft.com/net/tutorials/csharp/getting-started/hello-world) from [.NET Documentation](https://docs.microsoft.com/en-us/dotnet/)
Also, it doesn't explain how to write [XML Documentation Comments (C# Programming Guide)](https://msdn.microsoft.com/en-us/library/b2s063f7.aspx) which is like JavaDoc

.NET Core is a subset of .NET Framework and not all types and methods are available. And not all methods are really needed:
- ToShortDateString() is the same as ToString("d"), the rest of ToXString have similar equivalents
- TOADate() is unlikely to be of much use cross platform as OLE Automation Date is a Windows specific format.

For example, in this video, he uses C# with .NET Framework 
In 13 | Working with Dates and Times, When he run Console.WriteLine(myValue.ToShortDateString());,
he gets following error:  
`
'DateTime' does not contain a definition for 'ToShortDateString' and no extension method 'ToShortDateString' accepting a first argument of type 'DateTime' could be found (are you missing a using directive or an assembly reference?)
`  
but when I changed it to Console.WriteLine(myValue.ToString("d")), 
I got same output he got.

## List of userful methos for C#
#### Writes the text representation of the specified value or values to the standard output stream.
```
Console.Write()
```
#### Writes the current line terminator to the standard output stream.
```
WriteLine()
```
#### Converts string into an integer
```
int result = int.Parse(Console.ReadLine());
```
#### Converts the value of objects to strings based on the formats specified and inserts them into another string. For example, This method includes a format string with three format items, {0}, {1}, and {2}, and an argument list with three items below.
```
String.Format(String, Object, Object, Object) 
```
#### Clears the console buffer and corresponding console window of display information.
```
Console.Clear()
```
#### String format
```
Console.WriteLine(String.Format("{0:N}"), 1234567)  // 1,234,567,890.00 
Console.WriteLine(String.Format(("Percentage: {0:P}", .123))  //12.30 %
Console.WriteLine(String.Format("Phone Number {0:(###) ###-####}", 123456789012)  //Phone Number: (12345)678-9012
```
[More Standard Numeric Format Strings](https://msdn.microsoft.com/en-us/library/dwhawy9k(v=vs.110).aspx)

## List of the websites to learn C#
https://mva.microsoft.com/en-US/training-courses/c-fundamentals-for-absolute-beginners-16169?l=l5iWxYQIC_1306218949
https://www.microsoft.com/net/tutorials/csharp/getting-started
https://docs.microsoft.com/en-us/
