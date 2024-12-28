# Git Kurulumu
Git, bir komut satırı aracıdır. Git'i kurmaya başlayalım.

### Git Yüklü mü?
İlk olarak, Git'in zaten yüklü olup olmadığını kontrol edelim. Bir terminal açın ve şu komutu yazın:

```bash
git --version
```

Eğer bir sürüm numarası görüyorsanız, Git yüklü anlamına gelir ve versiyon bilgisine erişirsiniz.

Eğer Git yüklü değilse, aşağıdaki adımları izleyerek Git'i kurabilirsiniz.

---

## Git Kurulumu

### Windows (WSL) / Linux (Ubuntu)
Aşağıdaki komutu kullanarak Git'i yükleyebilirsiniz:

```bash
sudo apt install git-all
```

### Mac OS
Terminalde `git --version` komutunu çalıştırdığınızda, Git'i yüklemenizi isteyen bir uyarı alabilirsiniz. Eğer bu gerçekleşmezse, Homebrew kullanarak Git'i yükleyebilirsiniz:

```bash
brew install git
```

## Global Yapılandırma
Git'i yükledikten sonra, kullanıcı adınızı ve e-posta adresinizi ayarlamalısınız. Bu bilgiler, her commit işleminde kullanılacaktır.
Öncelikle zaten ayarlanmış bir kullanıcı adı ve e-posta adresi var mı kontrol edelim:

```bash
git config --get user.name
git config --get user.email
```

```bash
git config --add --global user.name "Adınız"
git config --add --global user.email "E-posta Adresiniz"
```
Burada:
* `git config` : Git yapılandırma komutu
* `--add` : Yapılandırma dosyasına yeni bir giriş ekler
* `--global` : Yapılandırma dosyasına global bir giriş ekler
* `user` : Kullanıcı yapılandırma seçeneği. Section olarak adlandırılır.
* `name` : Kullanıcı adı
----

Git hakkında detaylı bilgi edinmek için terminalde aşağıdaki komutu kullanabilirsiniz:

```bash
man git
```

