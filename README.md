# Desharp - C#/VB .NET Debugging Tool - Code Snippets
Visual Studio code snippets - automaticly generated code snippets from 3-4 letter shortcuts to work better with Desharp library.

## Shortcuts
- dumping:
  - **ddd** - Desharp.Debug.Dump(params object[] args); || Desharp.Debug.Dump(Exception exception = null, DumpOptions? options = null);
  - **dddd** - Desharp.Debug.DumpAndDie(object obj = null, DumpOptions? options = null);
  - **dddo** - Desharp.Debug.Dump(object obj, DumpOptions? options = null);
- logging
  - **dde** - Desharp.Debug.Log(Exception exception = null);
  - **ddl** - Desharp.Debug.Log(object obj = null, Level level = Level.INFO, int maxDepth = 0, int maxLength = 0);
- other
  - **dds** - Desharp.Debug.Stop();
  - **ddc** - Desharp.Debug.Configure(DebugConfig cfg);
  - **dda** - Desharp.Debug.Assert(bool assertion, string description = "", Level logLevel = Level.DEBUG);
  - **ddt** - Desharp.Debug.Timer(string name = null, bool returnTimerSeconds = false, Level logLevel = Level.DEBUG);


## Instalation
- download and unzip package
- copy all files from directory `Visual C#` with extension `.snippet` into directory:
  - for VS 2015 (x64): `C:\Program Files (x86)\Microsoft Visual Studio 14.0\VC#\Snippets\1033\Visual C#\`
  - for VS 2015 (x86): `C:\Program Files\Microsoft Visual Studio 14.0\VC#\Snippets\1033\Visual C#\`
  - for VS 2013 (x64): `C:\Program Files (x86)\Microsoft Visual Studio 12.0\VC#\Snippets\1033\Visual C#\`
  - for VS 2013 (x86): `C:\Program Files\Microsoft Visual Studio 12.0\VC#\Snippets\1033\Visual C#\`
  - ...
