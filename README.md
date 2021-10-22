# bad-code

I wanted to build an application that contains as many examples as possible of the bad code that will likely be encountered in the real world.

Once the app is built, it could be used by anyone for refactoring practise/teaching purposes.

I've been considering doing something with YouTube or Twitch so could possibly build the app and refactor it on a stream.

## What sins should it contain?
Will add to this list bad things that I want in the app. If anyone stumbles upon this repo and wants to add more ideas, feel free.

* 1000+ line long method containing lots of interwoven logic and state.
* Class with a number of public nested classes that are used elsewhere in the project for otherwise completely unrelated purposes.
* Impure projects (Domain project containing data access).
* Duplicate code, especially between connected and otherwise-unconnected projects. Include some "incidentally" identical code examples.
* Utils project, because every application has one.
* Objects that wrap other objects but also expose them publicly with other objects using them.
* Objects that take data in odd ways (datetimes or ints as string, multiple data points as a delimited list, etc).
* Accessing database using ADO, EF, and some hand-rolled data methods.
* Inapproprate accessibility (methods that should be private/internal exposed as publics).
* Example of replacing old with new but never really removing old, something like below where both implementations are used in different scenarios.
```csharp
if(useNew) {
    //Do the new thing
  }
  else
  {
    //Do the old thing
  }
}
```
* More...
