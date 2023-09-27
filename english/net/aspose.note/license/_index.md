---
title: Class License
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.License class. Provides methods to license the component
type: docs
weight: 350
url: /net/aspose.note/license/
---
## License class

Provides methods to license the component.

```csharp
public sealed class License
```

## Constructors

| Name | Description |
| --- | --- |
| [License](license/)() | Initializes a new instance of the `License` class. |

## Methods

| Name | Description |
| --- | --- |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense)(Stream) | Licenses the component. |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense_1)(string) | Licenses the component. |

## Examples

In this example, an attempt will be made to find a license file named MyLicense.lic in the folder that contains the component, in the folder that contains the calling assembly, in the folder of the entry assembly and then in the embedded resources of the calling assembly.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

Shows how to load a license for Aspose.Note from a file.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Shows how to load a license for Aspose.Note from a stream.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

Shows how to load a license for Aspose.Note from embedded file resource.

```csharp
// Instantiate the License class
Aspose.Note.License license = new Aspose.Note.License();

// Pass only the name of the license file embedded in the assembly
license.SetLicense("Aspose.Note.lic");
```

### See Also

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


