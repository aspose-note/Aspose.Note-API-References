---
title: License.SetLicense
second_title: Aspose.Note for .NET API Reference
description: License method. Licenses the component
type: docs
weight: 20
url: /net/aspose.note/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Licenses the component.

```csharp
public void SetLicense(string licenseName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| licenseName | String | Can be a full or short file name or name of an embedded resource. Use an empty string to switch to evaluation mode. |

## Remarks

Tries to find the license in the following locations:

1. Explicit path.

2. The folder that contains the Aspose component assembly.

3. The folder that contains the client's calling assembly.

4. The folder that contains the entry (startup) assembly.

5. An embedded resource in the client's calling assembly.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Explicit path.

2. An embedded resource in the client's calling assembly.

## Examples

Shows how to load a license for Aspose.Note from a file.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Shows how to load a license for Aspose.Note from embedded file resource.

```csharp
// Instantiate the License class
Aspose.Note.License license = new Aspose.Note.License();

// Pass only the name of the license file embedded in the assembly
license.SetLicense("Aspose.Note.lic");
```

### See Also

* class [License](../)
* namespace [Aspose.Note](../../license/)
* assembly [Aspose.Note](../../../)

---

## SetLicense(Stream) {#setlicense}

Licenses the component.

```csharp
public void SetLicense(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | A stream that contains the license. |

## Remarks

Use this method to load a license from a stream.

## Examples

Shows how to load a license for Aspose.Note from a stream.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

### See Also

* class [License](../)
* namespace [Aspose.Note](../../license/)
* assembly [Aspose.Note](../../../)


