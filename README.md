# Desharp - .NET Debugging Tool - C#/VB Code Snippets
Visual Studio code snippets for C# or Visual Basic to work much faster with Desharp library by 3 or 4 letter shortcuts.

## Shortcuts
#### Dumping:
```csharp
// Snippet shortcut: ddd
Desharp.Debug.Dump(params object[] args);
Desharp.Debug.Dump(Exception exception = null, Desharp.DumpOptions? options = null);

// Snippet shortcut: dddo
Desharp.Debug.Dump(object obj, DumpOptions? options = null);

// Snippet shortcut: ddf
Desharp.Debug.Fire.Log(object obj);

// Snippet shortcut: dddd
Desharp.Debug.DumpAndDie(object obj = null, DumpOptions? options = null);
```

```vb
' Snippet shortcut: ddd
Desharp.Debug.Dump(ParamArray args As Object)
Desharp.Debug.Dump(Optional exception As Exception = Nothing, Optional options As DumpOptions? = Nothing)

' Snippet shortcut: dddo
Desharp.Debug.Dump(obj As Object, Optional options As DumpOptions? = Nothing)

' Snippet shortcut: ddf
Desharp.Debug.Fire.Log(obj As Object)

' Snippet shortcut: dddd
Desharp.Debug.DumpAndDie(Optional obj As Object = Nothing, Optional options As DumpOptions? = Nothing)
```

#### Logging:
```cs
// Snippet shortcut: dde
Desharp.Debug.Log(Exception exception = null);

// Snippet shortcut: ddl
Desharp.Debug.Log(object obj = null, Level level = Level.INFO, int maxDepth = 0, int maxLength = 0);
```

```vb
' Snippet shortcut: dde
Desharp.Debug.Log(Optional exception As Exception)

' Snippet shortcut: ddl
Desharp.Debug.Log(
  Optional obj As Object = Nothing, 
  Optional level As Level = Level.INFO, 
  Optional maxDepth As Int32 = 0, 
  Optional maxLength As Int32 = 0
)
```

#### Other:
```cs
// Snippet shortcut: dds
Desharp.Debug.Stop();

// Snippet shortcut: ddc
Desharp.Debug.Configure(DebugConfig cfg);

// Snippet shortcut: dda
Desharp.Debug.Assert(bool assertion, string description = "", Level logLevel = Level.DEBUG);

// Snippet shortcut: ddt
Desharp.Debug.Timer(string name = null, bool returnTimerSeconds = false, Level logLevel = Level.DEBUG);
```

```vb
' Snippet shortcut: dds
Desharp.Debug.Stop()

' Snippet shortcut: ddc
Desharp.Debug.Configure(cfg As DebugConfig)

' Snippet shortcut: dda
Desharp.Debug.Assert(assertion As Boolean, Optional description As String = "", Optional logLevel As Level = Level.DEBUG)

' Snippet shortcut: ddt
Desharp.Debug.Timer(
  Optional name As String = Nothing, 
  Optional returnTimerSeconds As Boolean = False, 
  Optional logLevel As Level = Level.DEBUG
)
```

## Instalation - C#
- download and unzip package
- copy all files from repo directory `C#` with extension `.snippet` into directory:
  - for VS 2017: `C:\Program Files (x86)\Microsoft Visual Studio\2017\Enterprise\VC#\Snippets\1033\Visual C#\`
  - for VS 2017: `C:\Program Files (x86)\Microsoft Visual Studio 15.0\VC#\Snippets\1033\Visual C#\`
  - for VS 2015: `C:\Program Files (x86)\Microsoft Visual Studio 14.0\VC#\Snippets\1033\Visual C#\`
  - for VS 2013: `C:\Program Files (x86)\Microsoft Visual Studio 12.0\VC#\Snippets\1033\Visual C#\`
  - for VS 2012: `C:\Program Files (x86)\Microsoft Visual Studio 11.0\VC#\Snippets\1033\Visual C#\`
  - ...
- you can use it immediately, no needs to restart Visual Studio (tested in 2015)

## Instalation - Visual Basic
- download and unzip package
- copy all content from repo directory `Visual Basic` into directory:
  - for VS 2017: `C:\Program Files (x86)\Microsoft Visual Studio\2017\Enterprise\VB\Snippets\1033\other\`
  - for VS 2015: `C:\Program Files (x86)\Microsoft Visual Studio 14.0\VB\Snippets\1033\other\`
  - for VS 2013: `C:\Program Files (x86)\Microsoft Visual Studio 12.0\VB\Snippets\1033\other\`
  - for VS 2012: `C:\Program Files (x86)\Microsoft Visual Studio 11.0\VB\Snippets\1033\other\`
  - ...
- you can use it immediately, no needs to restart Visual Studio (tested in 2015)
