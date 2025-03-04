## **HOW**
1. *Mengunduh program wget, unzip, dan xxd dan membuat folder “artists_who_can_sing" lalu masuk kedalamnya.*
```
sudo apt update && sudo apt install wget unzip xxd -y && mkdir artists_who_can_sing && cd artists_who_can_sing
```
2. *Download file tutorial bernyanyi menggunakan wget, lalu unzip dan masukkan ke folder "singing_tutorials"*
```
wget --no-check-certificate "https://docs.google.com/uc?export=download&id=1lV1HVmPTY_BOAK6ToXymRu7V5eVfR0ut" -O tutorial.zip && unzip tutorial.zip -d singing_tutorials
```
3&4. *Masuk ke dalam folder dan tampilkan isinya (termasuk yang tersembunyi)
```
cd singing_tutorials && ls -la
```
5. Mencari tutorial "opera" by “NBAYoungboy” yang berisi "FLAG{}", kemudian redirect ke "flag.txt" di "artists_who_can_sing"
```
strings *opera*NBAY* | grep "FLAG{" > ../artists_who_can_sing/flag.txt
```
6. Buka folder sebelumnya dan download file baru bernama “plsrunmeiamnotmalwarefr”
```
cd .. && wget https://files.catbox.moe/9l4qu8 -O plsrunmeiamnotmalwarefr 
```
7. Mengubah izin untuk dapat meng-execute dan menjalankan program tersebut
```
chmod +x plsrunmeiamnotmalwarefr && ./plsrunmeiamnotmalwarefr
```
8. Melihat (proses) program yang baru dijalankan di atas^
```
ps aux | grep plsrunmeiamnotmalwarefr
```
9. Membuat file "ransom.moolah" lalu mengecek keadaan ransom-nya
```
touch ransom.moolah && ps aux

```
10. Menghentikan proses program lalu memastikan bahwa memang sudah berhenti
```
kill -9 $(ps -o ppid= -p <PID>)
```
11. Membuat user, memasukkan ke group, login user
```
sudo adduser yabadabadoo && sudo usermod -aG sudo yabadabadoo && groups yabadabadoo && su - yabadabadoo
```
12. Membuat folder, masuk ke dalamnya dan memastikan bahwa folder hanya dapat diakses oleh usernya dan root
```
mkdir fufufafa && cd fufufafa && sudo chmod 700 fufufafa
```
13. 
