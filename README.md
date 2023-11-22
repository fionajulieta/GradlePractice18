# GradlePractice18
Tugas module 18 : 
1. Buatlah Custom Task untuk melakukan perintah print “Hello Jayjay, My Name is <Student>”.
Nama Student boleh di hard code, namun cobalah cari bagaimana caranya melakukan passing parameter
pada Gradle CLI kedalam Gradle Task agar dapat membuat nama yang dynamic sesuai inputan
Referensi: https://www.baeldung.com/gradle-command-line-arguments
2. Tambahkan dependencies pada build.gradle file untuk library Selenium, Rest Assured dan Cucumber
3. Push semua perubahan pada repository

Ans:
- buat project baru di intellij idea dan pilih Gradle utk build systemnya
- utk add library, go to https://mvnrepository.com/ dan search selenium, rest assured, dan cucumber
- copy dependencynya trs paste didalam build.gradle >> dependencies{}
- click icon gradle utk sync
  
- Lalu untuk gradle tasknya, kita buat dengan syntax: task namaGradleTask(){ doLast {expression}}
- syntax -> variable = (condition) ? expressionTrue :  expressionFalse;

- untuk run tasknya, ketik di terminal: ./gradlew greetingTask -Pnama=<namakita>
- untuk hasil di attached screenshot, yg saya ketik di terminal adalah: ./gradlew greetingTask -Pnama=fiona

- terakhir di push ke github dari intellij nya:
    1. tambah remote repository: menu git > manage remotes > add new github url <https:// github.com/fionajulieta/GradlePractice18.git>
    2. menu git > add atau ketik 'git add .' di terminal
    3. menu git > commit directory > enter commentnya > klik commit
    4. menu git > push
