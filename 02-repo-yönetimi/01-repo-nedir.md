# Repository Nedir?

* Herhangi bir projenin ilk adımı bir repo oluşturmaktır. Bir Git "deposu" (veya "repo") tek bir projeyi temsil eder. Genellikle üzerinde çalıştığınız her proje için bir deponuz olur.

* Bir depo, esasen bir projeyi (diğer dizinleri ve dosyaları) içeren bir dizindir.

## Repo Oluşturma

* Bir dizin oluşuturup içine giriyoruz.

```bash
mkdir git-rehberi
cd git-rehberi
```

* Ardından `git init` komutu ile bu dizini bir git deposuna dönüştürüyoruz.

```bash
git init
```

* Kontrol etmek için `ls -a` komutunu kullanabiliriz.

```bash
ls -a
```
Bu gizli dizin, Git'in projeye ait tüm dahili izleme ve sürüm bilgilerini depoladığı yerdir.