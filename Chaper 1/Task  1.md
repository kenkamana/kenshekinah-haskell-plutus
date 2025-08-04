HC1T1 - Tâche 1 : Composition de fonctions
```haskell
-- Définition de la fonction double
double :: Int -> Int
double x = x * 2

-- Définition de la fonction increment
increment :: Int -> Int
increment x = x + 1

-- Composition des deux fonctions : double puis increment
doubleThenIncrement :: Int -> Int
doubleThenIncrement = increment . double

-- Exemple d'utilisation dans une fonction principale
main :: IO ()
main = do
    let valeur = 3
    let resultat = doubleThenIncrement valeur
    putStrLn ("Résultat : " ++ show resultat)
```

📌 **Explication rapide :**
- `double` multiplie un nombre par 2.
- `increment` l’augmente de 1.
- `doubleThenIncrement` applique d’abord `double`, puis `increment` grâce à l’opérateur de composition `(.)`.

