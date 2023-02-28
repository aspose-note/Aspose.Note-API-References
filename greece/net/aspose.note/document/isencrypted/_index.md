---
title: Document.IsEncrypted
second_title: Aspose.Note for .NET API Reference
description: Document μέθοδος. Ελέγχει εάν ένα έγγραφο από μια ροή είναι κρυπτογραφημένο. Για να το ελέγξουμε πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Επομένως αυτή η μέθοδος μπορεί να οδηγήσει σε ποινή απόδοσης.
type: docs
weight: 150
url: /el/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

Ελέγχει εάν ένα έγγραφο από μια ροή είναι κρυπτογραφημένο. Για να το ελέγξουμε πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Επομένως, αυτή η μέθοδος μπορεί να οδηγήσει σε ποινή απόδοσης.

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Η ροή. |
| options | LoadOptions | Οι επιλογές φόρτωσης. |
| document | Document& | Το φορτωμένο έγγραφο. |

### Επιστρεφόμενη Αξία

Επιστρέφει true εάν το έγγραφο είναι κρυπτογραφημένο αλλιώς false.

### Παραδείγματα

Δείχνει πώς μπορείτε να ελέγξετε εάν ένα έγγραφο προστατεύεται με κωδικό πρόσβασης.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Δείχνει πώς μπορείτε να ελέγξετε εάν ένα έγγραφο προστατεύεται με κωδικό πρόσβασης με συγκεκριμένο κωδικό πρόσβασης.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Δείτε επίσης

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

Ελέγχει εάν ένα έγγραφο από μια ροή είναι κρυπτογραφημένο. Για να το ελέγξουμε πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Επομένως, αυτή η μέθοδος μπορεί να οδηγήσει σε ποινή απόδοσης.

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Η ροή. |
| password | String | Ο κωδικός πρόσβασης για την αποκρυπτογράφηση ενός εγγράφου. |
| document | Document& | Το φορτωμένο έγγραφο. |

### Επιστρεφόμενη Αξία

Επιστρέφει true εάν το έγγραφο είναι κρυπτογραφημένο αλλιώς false.

### Παραδείγματα

Δείχνει πώς μπορείτε να ελέγξετε εάν ένα έγγραφο προστατεύεται με κωδικό πρόσβασης.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Δείχνει πώς μπορείτε να ελέγξετε εάν ένα έγγραφο προστατεύεται με κωδικό πρόσβασης με συγκεκριμένο κωδικό πρόσβασης.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Δείτε επίσης

* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

Ελέγχει εάν ένα έγγραφο από μια ροή είναι κρυπτογραφημένο. Για να το ελέγξουμε πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Επομένως, αυτή η μέθοδος μπορεί να οδηγήσει σε ποινή απόδοσης.

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Η ροή. |
| document | Document& | Το φορτωμένο έγγραφο. |

### Επιστρεφόμενη Αξία

Επιστρέφει true εάν το έγγραφο είναι κρυπτογραφημένο αλλιώς false.

### Παραδείγματα

Δείχνει πώς μπορείτε να ελέγξετε εάν ένα έγγραφο προστατεύεται με κωδικό πρόσβασης.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Δείχνει πώς μπορείτε να ελέγξετε εάν ένα έγγραφο προστατεύεται με κωδικό πρόσβασης με συγκεκριμένο κωδικό πρόσβασης.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Δείτε επίσης

* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

Ελέγχει εάν ένα έγγραφο από ένα αρχείο είναι κρυπτογραφημένο. Για να το ελέγξουμε πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Επομένως, αυτή η μέθοδος μπορεί να οδηγήσει σε ποινή απόδοσης.

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Η διαδρομή του αρχείου. |
| options | LoadOptions | Οι επιλογές φόρτωσης. |
| document | Document& | Το φορτωμένο έγγραφο. |

### Επιστρεφόμενη Αξία

Επιστρέφει true εάν το έγγραφο είναι κρυπτογραφημένο αλλιώς false.

### Παραδείγματα

Δείχνει πώς μπορείτε να ελέγξετε εάν ένα έγγραφο προστατεύεται με κωδικό πρόσβασης.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Δείχνει πώς μπορείτε να ελέγξετε εάν ένα έγγραφο προστατεύεται με κωδικό πρόσβασης με συγκεκριμένο κωδικό πρόσβασης.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Δείτε επίσης

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

Ελέγχει εάν ένα έγγραφο από ένα αρχείο είναι κρυπτογραφημένο. Για να το ελέγξουμε πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Επομένως, αυτή η μέθοδος μπορεί να οδηγήσει σε ποινή απόδοσης.

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Η διαδρομή του αρχείου. |
| document | Document& | Το φορτωμένο έγγραφο. |

### Επιστρεφόμενη Αξία

Επιστρέφει true εάν το έγγραφο είναι κρυπτογραφημένο αλλιώς false.

### Παραδείγματα

Δείχνει πώς μπορείτε να ελέγξετε εάν ένα έγγραφο προστατεύεται με κωδικό πρόσβασης.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Δείχνει πώς μπορείτε να ελέγξετε εάν ένα έγγραφο προστατεύεται με κωδικό πρόσβασης με συγκεκριμένο κωδικό πρόσβασης.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Δείτε επίσης

* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

Ελέγχει εάν ένα έγγραφο από ένα αρχείο είναι κρυπτογραφημένο. Για να το ελέγξουμε πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Επομένως, αυτή η μέθοδος μπορεί να οδηγήσει σε ποινή απόδοσης.

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Η διαδρομή του αρχείου. |
| password | String | Ο κωδικός πρόσβασης για την αποκρυπτογράφηση ενός εγγράφου. |
| document | Document& | Το φορτωμένο έγγραφο. |

### Επιστρεφόμενη Αξία

Επιστρέφει true εάν το έγγραφο είναι κρυπτογραφημένο αλλιώς false.

### Παραδείγματα

Δείχνει πώς μπορείτε να ελέγξετε εάν ένα έγγραφο προστατεύεται με κωδικό πρόσβασης.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Δείχνει πώς μπορείτε να ελέγξετε εάν ένα έγγραφο προστατεύεται με κωδικό πρόσβασης με συγκεκριμένο κωδικό πρόσβασης.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Δείτε επίσης

* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)


