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


### Kısaca Git ile ilgili kavramlar
### Key Concepts of Git (Briefly)


✅ Global config: Kullanıcı bilgilerini git sistemine kaydetmek için kullanılan konfigürasyonlar.
  *Configurations used to save user information in the Git system.*
  * Git'i kullanmaya başlamadan önce kullanıcı adı ve e-posta adresinizi ayarlamanız gerekiyor:
  *Before using Git, you need to set your username and email address.*

`git config --global user.name "Adınız Soyadınız"`


`git config --global user.email "epostanız@example.com"`



✅ Commit: Değişiklikleri benim değişimle bir paket haline getirip sonra bu paketin üstüne adres yazmak gibidir. Başka bir değişle yapılan bir değişikliğin kaydedilmesi işlemine denir. 
  
  *It is like bundling changes into a package with my changes and then writing an address on top of this package. This refers to the process of recording a change made by someone else.*

✅ Init : git versiyon sistemini başlatama işlemidir.
    
*It is the process of initializing the Git version control system.*

     
     `git init` 

✅ Status: git deposundaki anlık durumu göstermeye yarar.

  *It is used to show the current status of the Git repository.*

     git status

✅ Push : git uzak deposundaki genellikle github değişiklikleri yollamaya yarayan kod.

*It is the code used to send changes to the Git remote repository, typically on GitHub.*
    git push


✅ Pull : git deposundaki değişiklikleri makinana almaya yarar.
 
 *It is used to fetch changes from the Git repository to your machine.*

    git pull
✅ Branch: Bir projenin geliştirilmesi için ayrılan yollara branch denir. Ana yolumuza main ya da master branch denir.

*The paths allocated for the development of a project are called branches. The main path is referred to as the main or master branch.*
    
    `git branch branchadı`  
   
   bu kod ile yeni branch oluşturabilirsiniz.
   
   You can create a new branch with this code.

    `git checkout -b yeni-branch` 
   
   bu kod ile yeni-branche geçiş yapabilirsiniz.

   You can switch to the new branch with this code.

✅ Merge : Bir branch’in içindeki değişiklikleri başka bir branch’e dahil etmek için kullanılır
 
 *It is used to incorporate the changes from one branch into another branch.*
    
    `git merge mainbracheklenecekbranch` 
  
  bu kod default olarak mainde olduğunuz varsayılarak yazıldı.

  This code is written assuming that you are on the main branch by default.

✅ Rebase : bir branch’in değişikliklerini başka bir branch’in son commit’leri üzerine ekler. Merge göre daha temiz bir commit geçmişi ayarlar.

*It adds the changes of one branch onto the last commits of another branch. It creates a cleaner commit history compared to merge.*

    `git rebase main`
---
### Git stating nedir?

Git 3 aşamalı katmandan sistemiyle çalışmaktadır.

*Git works with a three-stage layering system.*
1. Working Directory (Çalışma Alanı) Bu alana projemizin dosylarını düzenlediğimiz alanda denilebilir.
  *1. Working Directory (Working Area) This can be considered as the area where we organize the files of our project.*
2. Staging Area (Hazırlık Alanı)  Burada commit atmadan önce hangi değişikliklerinin comite ekleneceğinin ayarlandığı bölümdür.
  This is the area where you configure which changes will be included in the commit before actually committing.
   * Belirli bir dosyayı comite eklemek için: To add a specific file to the commit:
   
     `git add dosyadı.dosyauzantısı`
   * Tüm değişiklikleri eklemek için: To add all changes:
   `git add .`
3. Repository (Depo): Commit edilen dosyaların Git tarafından kalıcı olarak saklandığı alan.
The area where the files that have been committed are stored permanently by Git.

### Bugrahan Bayrakci