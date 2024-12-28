# Merge

* Farklı branch'lerde yapılan değişiklikleri birleştirmek için kullanılır.

```bash
A - B - C    main
   \
    D - E    other_branch
```

```bash
A - B - C - F    main
   \     /
    D - E        other_branch
```

## Örnek Bir Senaryo

* `main` branch'ine geçelim ve `contents.md` dosyasını oluşturalım.

```bash
git switch main
```

```bash
nano contents.md
```

```bash
# contents

- titles.md: The movie titles in the WebFlyx collection
- quotes: A directory of files containing memorable quotes from movies
```

```bash
git add contents.md
git commit -m "D: Add contents.md"
```

*  `add_classics` branch'inde `contents.md` dosyasını güncelleyelim.

```bash
nano contents.md
```

```bash
# contents

- titles.md: The movie titles in the WebFlyx collection
- classics.csv: A comma-separated list of classic movies
- quotes: A directory of files containing memorable quotes from movies
```

```bash
git add contents.md
git commit -m "E: Add contents.md"
```

* `main` branch'ine geçelim ve `add_classics` branch'ini `main` branch'ine birleştirelim.

```bash
git switch main
```

```bash
git merge add_classics
```

```bash
git log --oneline --decorate --graph --parents
```

# Rebase

* Farklı branch'lerde yapılan değişiklikleri birleştirmek için kullanılır. Fakat `merge`'den farklı olarak, `rebase` işlemi sonucunda commit geçmişi değişir.

```bash
A - B - C    main
   \
    D - E    feature_branch
```

```bash
A - B - C         main
         \
          D - E   feature_branch
```


