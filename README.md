#My Prompt

# Tracks on Tracks on Tracks

Welcome to Tracks on Tracks on Tracks on Exercism's C# Track.
If you need help running the tests or submitting your code, check out `HELP.md`.
If you get stuck on the exercise, check out `HINTS.md`, but try and solve it without using those first :)

## Introduction

## Lists

Lists in C# are collections of primitive values or instances of structs or classes. They are implemented in the base class library as `List<T>` where `T` is the type of the item in the list. The API exposes a rich set of methods for creating and manipulating lists.

Items can be added to and removed from lists. They grow and shrink as necessary.

```csharp
var listOfStrings = new List<string>();
```

## Generic Types

A collection definition typically includes a place holder in angle brackets, often `T` by convention. Such a collection is referred to as a generic type. This allows the collection user to specify what type of items to store in the collection. In the above example code we are instantiating a list of strings.

## Instructions

In this exercise you'll be writing code to keep track of a list of programming languages you want to learn on Exercism.

You have nine tasks, which will all involve dealing with lists.

## 1. Create a new list

To keep track of the languages you want to learn, you'll need to create a new list.

Implement the static `Languages.NewList()` method that returns a new, empty list.

```csharp
Languages.NewList()
// => empty list
```

## 2. Define an existing list

Currently, you have a piece of paper listing the languages you want to learn: C#, Clojure and Elm.

Please implement the static `Languages.GetExistingLanguages()` method to return the list.

```csharp
Languages.GetExistingLanguages();
// => {"C#", "Clojure", "Elm"}
```

## 3. Add a new language to a list

As you explore Exercism and find more interesting languages, you want to add them to your list.

Implement the static `Languages.AddLanguage()` function to add a new language to the end of your list.

```csharp
Languages.AddLanguage(Languages.GetExistingLanguages(), "VBA");
// => {"C#", "Clojure", "Elm", "VBA"}
```

## 4. Count the languages in the list

Counting the languages one-by-one is inconvenient.

Implement the static `Languages.CountLanguages()` method to count the number of languages on your list.

```csharp
Languages.CountLanguages(Languages.GetExistingLanguages())
// => 3
```

## 5. Check to see if a language is in the list

Implement the static `Languages.HasLanguage()` method to check if a language is present.

```csharp
Languages.HasLanguage(Languages.GetExistingLanguages(), "Elm")
// => true
```

## 6. Reverse the list

At some point, you realize that your list is actually ordered backwards!

Implement the static `Languages.ReverseList()` method to reverse your list.

```csharp
Languages.ReverseList(Languages.GetExistingLanguages())
// => {"Elm", "Clojure", "C#"}
```

## 7. Check if list is exciting

While you love all languages, C# has a special place in your heart. As such, you're really excited about a list of languages if:

- The first on the list is C#.
- The second item on the list is C# and the list contain either two or three languages.

Implement the static `Languages.IsExciting()` method to check if a list of languages is exciting:

```csharp
Languages.IsExciting(Languages.GetExistingLanguages())
// => true
```

## 8.Remove Language

Please implement the static `Languages.RemoveLangage()` method to remove a specified language from the list.

```csharp
Languages.RemoveLanguage(Languages.GetExistingLanguages(), "Clojure")
// => { "C#", "Elm" }
```

## 9. Check if all languages in the list are unique

Please implement the static `Languages.IsUnique()` method to check if any of the languages is repeated in the list.

The list of languages (i.e. the parameter) is guaranteed not to be empty when this method is called and it doesn't matter if the list is modified.

```csharp
Languages.IsUnique(Languages.GetExistingLanguages())
// => true
```

## Source

### Created by

- @mikedamay

### Contributed to by

- @ErikSchierboom
- @yzAlvin
- @sanderploegsma
