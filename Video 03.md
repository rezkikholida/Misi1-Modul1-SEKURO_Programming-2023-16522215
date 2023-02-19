# #3 GITHUB : BRANCH

## Istilah yang digunakan

**Branch** yaitu jalur 'development' bebeas dari sebuah commit. Branching dilakukan untuk membuat snapshot tanpa mengganggu jalur utama, atau bisa juga sebagai fitur eksperimental.
**Checkout** yaitu berpindah ke branch / commit yang lain.
**Pull Request** yaitu meminta pemilik repository untuk 'mengambil' perubahan yang telah dilakukan.
**Merge** yaitu menggabungkan 2 branch.
**Merge Conflict** terjadi ketika baris yang sama diubah oleh 2 branch yang berbeda.

## Langkah membuat Branch

Buka file yang akan di-branching.

![01](https://user-images.githubusercontent.com/124449052/219933611-d1491023-4a22-4180-9eff-a31513b4f3f3.png)

Cara melakukan branch ada dua cara:

1.	Edit file terlebih dahulu, baru kemudian saat commit pilih new branch

![02](https://user-images.githubusercontent.com/124449052/219933614-95ed40fd-2597-4130-bebe-f2b01b77e067.png)

2.	Membuat branch dulu, lalu switch ke branch tersebut, baru melakukan edit

![03](https://user-images.githubusercontent.com/124449052/219933616-512fa85c-ba7d-4356-ae80-ae2bd0e83ffa.png)


Saat ini sudah terdapat branch baru bernama **daftar’**

![04](https://user-images.githubusercontent.com/124449052/219933621-09954122-0570-4c9a-b6dc-4d4f5cc5f842.png)

Switch branch ke **daftar’** kemudian buat file baru.

![05](https://user-images.githubusercontent.com/124449052/219933624-80f4af75-99e6-4eb2-a23c-5f747343a8ab.png)

Saat melakukan commit, akan muncul opsi **Commit directly to the *daftar’* branch**.

![06](https://user-images.githubusercontent.com/124449052/219933627-b1b5cf09-60d2-4e9f-89e7-9f5f5a513852.png)

Klik **Commit new file**.

Akan muncul tampilan sebagai berikut:

![07](https://user-images.githubusercontent.com/124449052/219933602-cfdd1b97-18e6-4758-926a-de69586c8d4f.png)

Jika kita pindah ke **main** branch, file **daftar (bukan makanan).md** tidak terdapat di dalamnya. 

![08](https://user-images.githubusercontent.com/124449052/219933604-058d976c-cead-450d-b7c4-15ef5c7b2dac.png)

Jadi, jika dilakukan perubahan pada branch **daftar’**, branch **main** tidakakan terpengaruh.

Tampilan pada network menjadi seperti berikut:

![09](https://user-images.githubusercontent.com/124449052/219933606-5bf8b058-394d-470a-8c12-e4681b329a8c.png)



## Melakukan Merge

Pada tampilan di bawah, klik **Compare & pull request**.

![10](https://user-images.githubusercontent.com/124449052/219933608-92af3e37-ae41-4717-baf2-2cdf7a81bd87.png)

Jika tidak ada baris yang conflict, akan muncul tampilan sebagai berikut dan git bisa melakukan merging secara otomatis. Jika ada baris yang conflict, git tidak bisa melakukan merge secara otomatis, namun kita masih dapat mengajukan pull request. Merging akan dilakukan secara manual dengan mengubah bagian yang conflict sesuai keinginan pemilik repo.

![11](https://user-images.githubusercontent.com/124449052/219933610-f459678c-7d02-49fe-bc16-c8f86269ca6d.png)

Tuliskan pesan lalu klik **Create a pull request**.

![12](https://user-images.githubusercontent.com/124449052/219933825-8d9ea63a-52f4-48bc-9b81-5dc9d797639d.png)

Setelah itu, kita akan diarahkan ke tab **Pull requests**.

![13](https://user-images.githubusercontent.com/124449052/219933826-a71b0496-025d-45be-9d76-c0bc853b7729.png)

Jika beralih dari tab **Code** ke tab **Pull requests**, akan muncul tampilan sebagai berikut. Klik file tersebut dan akan muncul tampilan seperti di atas.

![14](https://user-images.githubusercontent.com/124449052/219933827-71097b82-264d-4638-af67-b0b9ec1a3355.png)

Scroll ke bawah. Jika tidak ada baris yang conflict, kita bias langsung melakukan merge. Klik **Merge pull request**. Namun, jika ada baris yang conflict, merge harus diselesaikan dulu dengan cara manual.

![15](https://user-images.githubusercontent.com/124449052/219933828-1f21eda6-76b2-44e7-bf18-6d8dd4a225c2.png)

Klik **Confirm merge**.

![16](https://user-images.githubusercontent.com/124449052/219933829-d36e6ab7-033e-4ba6-9af5-35354e776efe.png)

Jika sudah berhasil melakukan merge, akan muncul tampilan seperti ini:

![17](https://user-images.githubusercontent.com/124449052/219933831-070437dd-c63f-4416-bbb2-6945f7160c38.png)

Angka pada tab **Pull requests** akan berkurang 1 karena satu file sudah di-merge. Jika dicek pada Network (terdapat pada tab Insights), dapat dilihat bahwa branch **daftar’** bergabung dengan branch **main**. Ini disebut fast-forward merging. Jika terda[at baris conflict, karena kita melakukan resolve terlebih dahulu, yang terjadi adalah three-way merging.

![18](https://user-images.githubusercontent.com/124449052/219933832-9d8a7c1f-c698-4b14-b7c8-1e17908b0ed4.png)
