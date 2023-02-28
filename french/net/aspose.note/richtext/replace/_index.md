---
title: RichText.Replace
second_title: Référence de l'API Aspose.Note pour .NET
description: RichText méthode. Remplace toutes les occurrences dun caractère Unicode spécifié dans cette instance par un autre caractère Unicode spécifié.
type: docs
weight: 200
url: /fr/net/aspose.note/richtext/replace/
---
## Replace(char, char) {#replace}

Remplace toutes les occurrences d'un caractère Unicode spécifié dans cette instance par un autre caractère Unicode spécifié.

```csharp
public RichText Replace(char oldChar, char newChar)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| oldChar | Char | L'ancien car. |
| newChar | Char | Le nouveau car. |

### Return_Value

Le[`RichText`](../) .

### Voir également

* class [RichText](../)
* espace de noms [Aspose.Note](../../richtext/)
* Assemblée [Aspose.Note](../../../)

---

## Replace(string, string) {#replace_1}

Remplace toutes les occurrences d'une chaîne spécifiée dans l'instance actuelle par une autre chaîne spécifiée.

```csharp
public RichText Replace(string oldValue, string newValue)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| oldValue | String | L'ancienne valeur. |
| newValue | String | La nouvelle valeur. |

### Return_Value

Le[`RichText`](../) .

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### Exemples

Montre comment parcourir le texte de la page et effectuer un remplacement.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Récupère tous les nœuds RichText
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Remplace le texte d'une forme
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Enregistrer dans n'importe quel format de fichier pris en charge
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Montre comment générer un nouveau document en remplaçant des morceaux de texte spéciaux dans un modèle.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var D = new Dictionary<string, string>
            {
                { "Company", "Atlas Shrugged Ltd" },
                { "CandidateName", "John Galt" },
                { "JobTitle", "Chief Entrepreneur Officer" },
                { "Department", "Sales" },
                { "Salary", "123456 USD" },
                { "Vacation", "30" },
                { "StartDate", "29 Feb 2024" },
                { "YourName", "Ayn Rand" }
            };

// Charge le modèle de document dans Aspose.Note.
var d = new Document(Path.Combine(dataDir, "JobOffer.one"));

// Remplaçons tous les mots du modèle
foreach (var e in d.GetChildNodes<RichText>())
{
    foreach (var replace in D)
    {
        e.Replace($"${{{replace.Key}}}", replace.Value);
    }
}

d.Save(Path.Combine(dataDir, "JobOffer_out.one"));
```

### Voir également

* class [RichText](../)
* espace de noms [Aspose.Note](../../richtext/)
* Assemblée [Aspose.Note](../../../)

---

## Replace(string, string, TextStyle) {#replace_2}

Remplace toutes les occurrences d'une chaîne spécifiée dans l'instance actuelle par une autre chaîne spécifiée dans le style spécifié.

```csharp
public RichText Replace(string oldValue, string newValue, TextStyle style)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| oldValue | String | L'ancienne valeur. |
| newValue | String | La nouvelle valeur. |
| style | TextStyle | Le style de la nouvelle valeur. |

### Return_Value

Le[`RichText`](../) .

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### Voir également

* class [TextStyle](../../textstyle/)
* class [RichText](../)
* espace de noms [Aspose.Note](../../richtext/)
* Assemblée [Aspose.Note](../../../)


