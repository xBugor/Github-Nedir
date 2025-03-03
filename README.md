# Git ve GitHub Nedir?

Git
--

- ✅ Git bir <a href="#bilgi-kısmı">versiyon kontrol</a> sistemidir. 

   *Git a version control system.*
   
- ✅Yazılım geliştirme sürecinde dosyaların zaman içindeki değişikliklerini takip etmenizi sağlar.

  *It helps track changes made to files in a project over time*
- ✅Git, dosyalarınızı yerel bir depo içinde saklar. Buna repository denir. 

   *Git stores your files in a local repository called a repository.*
- ✅Her yapılan değişikliğe bir "**commit**" olarak kaydedilir. 

    *Every change is recorded as a "**commit**".*

- ✅Kodun farklı özelliklerinde veya ekip içerisinde farklı bölümlerinde çalışmak için " **branch**" denilen dallar oluşturulur.
  
  *When working on different sections or features of the project, **branches** are created to manage separate workstreams.*

- ✅Her geliştirici için projenin tam kopyası makinesinde bulunur.
  
  *Each developer has an exact copy of the project on their local machine.*

- ✅Git ile çevrimdışı çalışabilirsiniz.
 
  *Git allows you to work offline.*

<h4 id="bilgi-kısmı">🔖Versiyon kontrol: Projenizin her değişikliğini kayıt altına alıp daha sonra eski haline dönmenizi sağlayacaktır.</h4>

 
### Özetle 

 Git projelerinizi yerel olarak kontrol etmenizi sağlar.

# GitHub
- GitHub geliştiricilerin kodlarını depoladığı, yayınladığı uzak bir depodur.

  *GitHub is a remote repository where developers store and publish their code.*

- Git versiyon sistemi ile çalışmaktadır.
 
  *It works with the Git version control system.*

- Public olan projeleri indirip kullanabilirsiniz.

   *You can download and use public projects.*

- GitHub açık kaynak yazılımlar için kullanılan bir platform olduğu gibi özel projeler içinde kullanılabilir.

   GitHub is a platform used for open-source software, but it can also be used for private projects.*

- GitHub'a projeleri yüklemek için repository dediğimiz depoları açmak gereklidir.

  *To upload projects to GitHub, it is necessary to create repositories, which are called 'repos'.*


- Yazılımcılar için bir cv niyetindende kullanılabilir.
 
   *It can also be used as a CV for developers.*


# Kısaca Git ile ilgili kavramlar

✅ Global config: Kullanıcı bilgilerini git sistemine kaydetmek için kullanılan konfigürasyonlar.
  * Git'i kullanmaya başlamadan önce kullanıcı adı ve e-posta adresinizi ayarlamanız gerekiyor:

`git config --global user.name "Adınız Soyadınız"`


`git config --global user.email "epostanız@example.com"`



✅ Commit: Değişiklikleri benim değişimle bir paket haline getirip sonra bu paketin üstüne adres yazmak gibidir. Başka bir değişle yapılan bir değişikliğin kaydedilmesi işlemine denir. 

✅ Init : git versiyon sistemini başlatama işlemi nedir. Bashte

     `git init` yazarak kullanabilirsiniz.

✅ Status: git deposundaki anlık durumu göstermeye yarar.

     git status

✅ Push : git uzak deposundaki genellikle github değişiklikleri yollamaya yarayan kod.

    git push


✅ Pull : git deposundaki değişiklikleri makinana almaya yarar.

    git pull
✅ Branch: Bir projenin geliştirilmesi için ayrılan yollara branch denir. Ana yolumuza main ya da master branch denir.

    `git branch branchadı`  
   
   bu kod ile yeni branch oluşturabilirsiniz.

    `git checkout -b yeni-branch` 
   
   bu kod ile yeni-branche geçiş yapabilirsiniz.

✅ Merge : Bir branch’in içindeki değişiklikleri başka bir branch’e dahil etmek için kullanılır

    `git merge mainbracheklenecekbranch` 
  
  bu kod default olarak mainde olduğunuz varsayılarak yazıldı.

✅ Rebase : bir branch’in değişikliklerini başka bir branch’in son commit’leri üzerine ekler. Merge göre daha temiz bir commit geçmişi ayarlar.

    `git rebase main`
---
### Git stating nedir?

Git 3 aşamalı katmandan sistemiyle çalışmaktadır.

1. Working Directory (Çalışma Alanı) Bu alana projemizin dosylarını düzenlediğimiz alanda denilebilir.
2. Staging Area (Hazırlık Alanı)  Burada commit atmadan önce hangi değişikliklerinin comite ekleneceğinin ayarlandığı bölümdür.
   * Belirli bir dosyayı comite eklemek için:
   `git add dosyadı.dosyauzantısı`
   * Tüm değişiklikleri eklemek için:
   `git add .`
3. Repository (Depo): Commit edilen dosyaların Git tarafından kalıcı olarak saklandığı alan.


### Bugrahan Bayrakci