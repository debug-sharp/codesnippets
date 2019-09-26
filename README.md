# Desharp - .NET Debugging Tool - C#/VB Code Snippets

-----------------------------------------------

Visual Studio code snippets for C# or Visual Basic to work much faster with Desharp library by 3 or 4 letter shortcuts.

## Outline
- [Shortcuts](#shortcuts)
  - [Dumping](#dumping)
  - [Logging](#logging)
  - [Other](#other)
- [Instalation](#instalation)
- [How To Create Custom Code Snippet](#how-to-create-custom-code-snippet)

-----------------------------------------------

## Shortcuts

### Dumping

#### C#

```csharp
// shortcut:  ddd
// method:    Desharp.Debug.Dump(params object[] args);
// method:    Desharp.Debug.Dump(Exception exception = null, Desharp.DumpOptions? options = null);
Desharp.Debug.Dump(obj);

// shortcut:  dddo
// method:    Desharp.Debug.Dump(object obj, DumpOptions? options = null);
Desharp.Debug.Dump(obj, new Desharp.DumpOptions {
  Depth = 4,
  Return = false
});

// shortcut:  ddf
// method:    Desharp.Debug.Fire.Log(object obj);
Desharp.Debug.Fire.Log(obj);

// shortcut:  dddd
// method:    Desharp.Debug.DumpAndDie(object obj = null, DumpOptions? options = null);
Desharp.Debug.DumpAndDie(obj);
```

#### Visual Basic
```vb
' shortcut:   ddd
' method:     Desharp.Debug.Dump(ParamArray args As Object)
' method:     Desharp.Debug.Dump(
'               Optional exception As Exception = Nothing, 
'               Optional options As DumpOptions? = Nothing
'             )
Desharp.Debug.Dump(obj)

' shortcut:   dddo
' method:     Desharp.Debug.Dump(obj As Object, Optional options As DumpOptions? = Nothing)
Desharp.Debug.Dump(obj, New Desharp.DumpOptions With {
  .Depth = 4,
  .Return = false
})

' shortcut:   ddf
' method:     Desharp.Debug.Fire.Log(obj As Object)
Desharp.Debug.Fire.Log(obj)

' shortcut:   dddd
' method:     Desharp.Debug.DumpAndDie(
'               Optional obj As Object = Nothing, 
'               Optional options As DumpOptions? = Nothing
'             )
Desharp.Debug.DumpAndDie(obj)
```

### Logging

#### C#
```cs
// shortcut:  dde
// method:    Desharp.Debug.Log(Exception exception = null);
Desharp.Debug.Log(ee);

// shortcut:  ddl
// method:    Desharp.Debug.Log(
//              object obj = null, 
//              Level level = Level.INFO, 
//              int maxDepth = 0, 
//              int maxLength = 0
//            );
Desharp.Debug.Log(obj, Desharp.Level.DEBUG);
```

#### Visual Basic
```vb
' shortcut:   dde
' method:     Desharp.Debug.Log(Optional exception As Exception)
Desharp.Debug.Log(ee)

' shortcut:   ddl
' method:     Desharp.Debug.Log(
'               Optional obj As Object = Nothing, 
'               Optional level As Level = Level.INFO, 
'               Optional maxDepth As Int32 = 0, 
'               Optional maxLength As Int32 = 0
'             )
Desharp.Debug.Log(obj, Desharp.Level.DEBUG)
```

### Other

#### C#
```cs
// shortcut:  dds
// method:    Desharp.Debug.Stop();
Desharp.Debug.Stop();

// shortcut:  ddc
// method:    Desharp.Debug.Configure(Desharp.DebugConfig cfg);
Desharp.Debug.Configure(new Desharp.DebugConfig {
  Enabled = true,
  Depth = 3,
  Directory = "~/logs",
  LogFormat = Desharp.LogFormat.Auto
});

// shortcut:  dda
// method:    Desharp.Debug.Assert(bool assertion, string description = "", Level logLevel = Level.DEBUG);
Desharp.Debug.Assert(
  true,
  ""
);

// shortcut:  ddt
// method:    Desharp.Debug.Timer(string name = null, bool returnTimerSeconds = false, Level logLevel = Level.DEBUG);
Desharp.Debug.Timer("default");
```
#### Visual Basic
```vb
' shortcut:   dds
' method:     Desharp.Debug.Stop()
Desharp.Debug.Stop()

' shortcut:   ddc
' method:     Desharp.Debug.Configure(cfg As Desharp.DebugConfig)
Desharp.Debug.Configure(New Desharp.DebugConfig With {
  .Enabled = true,
  .Depth = 3,
  .Directory = "~/logs",
  .LogFormat = Desharp.LogFormat.Auto
})

' shortcut:   dda
' method:     Desharp.Debug.Assert(
'               assertion As Boolean, Optional description As String = "", 
'               Optional logLevel As Level = Level.DEBUG
'             )
Desharp.Debug.Assert(
  True,
  ""
)

' shortcut:   ddt
' method:     Desharp.Debug.Timer(
'               Optional name As String = Nothing, 
'               Optional returnTimerSeconds As Boolean = False, 
'               Optional logLevel As Level = Level.DEBUG
'             )
Desharp.Debug.Timer("default")
```

-----------------------------------------------

## Instalation

#### C#
- download and unzip package
- copy all files from repo directory `C#` with extension `.snippet` into directory:
  - for VS 2019: `%USERPROFILE%\Documents\Visual Studio 2019\Code Snippets\Visual C#\My Code Snippets\`
  - for VS 2017: `%USERPROFILE%\Documents\Visual Studio 2017\Code Snippets\Visual C#\My Code Snippets\`
  - for VS 2015: `%USERPROFILE%\Documents\Visual Studio 2015\Code Snippets\Visual C#\My Code Snippets\`
  - for VS 2013: `%USERPROFILE%\Documents\Visual Studio 2013\Code Snippets\Visual C#\My Code Snippets\`
				 `C:\Program Files (x86)\Microsoft Visual Studio 12.0\VC#\Snippets\1033\Visual C#\`
  - for VS 2012: `%USERPROFILE%\Documents\Visual Studio 2012\Code Snippets\Visual C#\My Code Snippets\`
				 `C:\Program Files (x86)\Microsoft Visual Studio 11.0\VC#\Snippets\1033\Visual C#\`
  - ...
- you can use it immediately, no needs to restart Visual Studio (tested in 2015+)

#### Visual Basic
- download and unzip package
- copy all content from repo directory `Visual Basic` into directory:

  - for VS 2019: `%USERPROFILE%\Documents\Visual Studio 2019\Code Snippets\Visual Basic\My Code Snippets\`
  - for VS 2017: `%USERPROFILE%\Documents\Visual Studio 2017\Code Snippets\Visual Basic\My Code Snippets\`
  - for VS 2015: `%USERPROFILE%\Documents\Visual Studio 2015\Code Snippets\Visual Basic\My Code Snippets\`
  - for VS 2013: `%USERPROFILE%\Documents\Visual Studio 2013\Code Snippets\Visual Basic\My Code Snippets\`
				 `C:\Program Files (x86)\Microsoft Visual Studio 12.0\VB\Snippets\1033\other\`
  - for VS 2012: `%USERPROFILE%\Documents\Visual Studio 2012\Code Snippets\Visual Basic\My Code Snippets\`
				 `C:\Program Files (x86)\Microsoft Visual Studio 11.0\VB\Snippets\1033\other\`
  - ...
- you can use it immediately, no needs to restart Visual Studio (tested in 2015+)

-----------------------------------------------

## How To Create Custom Code Snippet

https://docs.microsoft.com/en-us/visualstudio/ide/walkthrough-creating-a-code-snippet?view=vs-2019
