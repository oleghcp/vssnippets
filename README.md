# Snippets for Visual Studio

Place snippet files to snippet folder in addition to existing ones.  
For example for vs 2022 it is:  
`C:\Program Files\Microsoft Visual Studio\2022\Community\VC#\Snippets\1033\Visual C#\`

## Common C# Snippets

### Method

![](https://raw.githubusercontent.com/oleghcp/vssnippets/master/_images/mtod.png)

```
void MyMethod()
{
    throw new System.NotImplementedException();
}
```

### Yield return

![](https://raw.githubusercontent.com/oleghcp/vssnippets/master/_images/yr.png)

```csharp
yield return null;
```

### fixed

![](https://raw.githubusercontent.com/oleghcp/vssnippets/master/_images/fixed.png)

```csharp
fixed (void* ptr = value)
{

}
```

### StructLayout

![](https://raw.githubusercontent.com/oleghcp/vssnippets/master/_images/sl.png)

```csharp
[StructLayout(LayoutKind.Sequential, Pack = 1)]
```

### MethodImpl

![](https://raw.githubusercontent.com/oleghcp/vssnippets/master/_images/mi.png)

```csharp
[MethodImpl(MethodImplOptions.AggressiveInlining)]
```

## For Unity

### Debug.Log();

![](https://raw.githubusercontent.com/oleghcp/vssnippets/master/_images/dl.png)

```csharp
Debug.Log();
```

### SerializeField

![](https://raw.githubusercontent.com/oleghcp/vssnippets/master/_images/sf.png)

```csharp
[SerializeField]
```

### UnityObject

![](https://raw.githubusercontent.com/oleghcp/vssnippets/master/_images/uo.png)

```csharp
using UnityObject = UnityEngine.Object;
```

### #if UNITY_EDITOR

![](https://raw.githubusercontent.com/oleghcp/vssnippets/master/_images/ifue.png)

```csharp
#if UNITY_EDITOR

#endif
```

### #if UNITY_EDITOR || DEVELOPMENT_BUILD

![](https://raw.githubusercontent.com/oleghcp/vssnippets/master/_images/ifdb.png)

```csharp
#if UNITY_EDITOR || DEVELOPMENT_BUILD

#endif
```

### OnValidate + Reset

![](https://raw.githubusercontent.com/oleghcp/vssnippets/master/_images/vld.png)

```csharp
#if UNITY_EDITOR
    private void OnValidate()
    {
        ValidateData();
    }

    private void Reset()
    {
        ValidateData();
    }

    private void ValidateData()
    {

    }
#endif
```

### CustomEditor

![](https://raw.githubusercontent.com/oleghcp/vssnippets/master/_images/ce.png)

```csharp
[CustomEditor(typeof(ExampleClass))]
```

##  CustomPropertyDrawer

![](https://raw.githubusercontent.com/oleghcp/vssnippets/master/_images/cpd.png)

```csharp
[CustomPropertyDrawer(typeof(CustomType))]
```

### MethodButtonsEditor

Is used for `InspectorButtonAttribute` from https://github.com/oleghcp/UnityTools

![](https://raw.githubusercontent.com/oleghcp/vssnippets/master/_images/be.png)

```csharp
#if UNITY_EDITOR
    [UnityEditor.CustomEditor(typeof(ExampleClass)), UnityEditor.CanEditMultipleObjects]
    private class Editor : OlegHcpEditor.MethodButtonsEditor { }
#endif
```
