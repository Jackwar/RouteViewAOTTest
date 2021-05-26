Test to show inheriting RouteView for a custom inplementation throws a runtime error when using AOT with .NET 6 Preview 4.

RouteView in App.razor is replaced with the TestRouteView class that inherits RouteView. Change App.razor back to RouteView to subvert the error.

The thrown runtime error:  

crit: Microsoft.AspNetCore.Components.WebAssembly.Rendering.WebAssemblyRenderer[100]
      Unhandled exception rendering component: The type 'RouteViewAOTTest.TestRouteView' declares a parameter matching the name 'RouteData' that is not public. Parameters must be public.
System.InvalidOperationException: The type 'RouteViewAOTTest.TestRouteView' declares a parameter matching the name 'RouteData' that is not public. Parameters must be public.
