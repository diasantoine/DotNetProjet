# P2 - Fix an App (.NET)

Application e-commerce ASP.NET Core MVC (projet OpenClassrooms). L'objectif était d'identifier et corriger des bugs dans le panier, le service produit, la validation de commande et le service de langue.

## Prérequis

- Visual Studio (avec la charge de travail ASP.NET et développement web)

## Lancer l'application

1. Cloner le dépôt et ouvrir `P2FixAnAppDotNetCode.sln` dans Visual Studio
2. Dans l'Explorateur de solutions, faire un clic droit sur `P2FixAnAppDotNetCode` et sélectionner **Définir comme projet de démarrage**
3. Appuyer sur **F5** pour lancer avec IIS Express en mode débogage, ou **Ctrl+F5** pour lancer sans débogueur

Le navigateur s'ouvre automatiquement sur l'application.

## Bugs corrigés

| Branche | Correction |
|---|---|
| `fix/product-service` | Type de retour changé de tableau en `List<T>`, implémentation de `GetProductById` et `UpdateProductQuantities` |
| `fix/cart` | Implémentation de `AddItem`, `GetTotalValue`, `GetAverageValue` et `FindProductInCartLines` |
| `fix/order-validation` | Ajout des messages de validation localisés sur le modèle Order et dans le formulaire |
| `fix/language-service` | Implémentation de `SetCulture` et correction des cultures supportées dans `Startup.cs` |
| `creation-README` | Ajout du README avec prérequis, instructions de lancement et description des branches |
| `clean-comments` | Suppression du code commenté inutile et du logger non utilisé dans `ProductService` |

## Langues supportées

L'application supporte trois langues, sélectionnables depuis l'interface :

- Français (par défaut)
- Anglais
- Espagnol
