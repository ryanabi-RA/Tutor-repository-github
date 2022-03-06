# Tutorial Membuat repository Github
cara membuat repository otomatis dari localhost ke repository ke website github 

## 1. Melakukan autentikasi username dan email
```
git config --global user.name "user"
git config --global user.email "user@gmail.com"
```
## 2. melakukan scan seluruh file dan folder
```
git init
```
## 3. Cek status file yang sudah di add dan tidak
```
git status
```
## 4. menambahkan file atau keseluruhan file project

add Spesifik file
```
git add filename
```
or add all file
```
git add .
```

## 5. commit memberi identitas jalannya project
```
git commit -m "tes"
```
## 6. membuat reponya sesuaikan tulisan usergithubmu dan namareponya
```
curl -u 'usergithub':'token-api' https://api.github.com/user/repos -d '{"name":"nama-reponya","private":false}'
```
## 7. melakukan remote  repositories dari github ke localhost
```
git remote add origin git@github.com:usergithubmu/namareponya.git
```
## 8. untuk mengganti akses remote repositories baru
```
git remote set-url origin git@github.com:usergithubmu/nama-reponya.git
```
## 9. push ke github
```
git push -u origin master
```
