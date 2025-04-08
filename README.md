Nama : Muhammad Alif Pratama
Kelas : TK2B
Nim : 09030582428065

1. Eksekusi profil

   a).Edit file profile /etc/profile dan tampilkan pesan

   ![Cuplikan layar 2025-03-25 222502](https://github.com/user-attachments/assets/e10e9e86-f799-48f3-9016-f3bf308034bb)

   b).Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap file tersebut, cantumkan instruksi echo.
 
   ![Cuplikan layar 2025-03-25 223340](https://github.com/user-attachments/assets/12eb9eed-b082-4cf8-a2b8-e21a7900e1cf)

   ![Cuplikan layar 2025-03-25 223842](https://github.com/user-attachments/assets/35276189-6b96-4c95-b9a5-4c0ea33d775f)

   ![Cuplikan layar 2025-03-25 223956](https://github.com/user-attachments/assets/61ebf4a6-0d8c-4b18-8341-5382977f8fcf)

   ![Cuplikan layar 2025-03-25 224141](https://github.com/user-attachments/assets/09145c48-36bf-4160-a20d-5dfdbaf31c4c)
   
   c). -Instruksi su alifpratama dan exit
  ![Cuplikan layar 2025-03-25 224325](https://github.com/user-attachments/assets/14e20e4b-5222-4fcd-adbb-a112da2366fd)
       -instruksi su - alifpratama dan exit
  ![Cuplikan layar 2025-03-25 224522](https://github.com/user-attachments/assets/30d194b2-ca08-4d57-b31e-355791131a3d)
  Perbedaanya :
terletak pada bagaimana lingkungan pengguna dikonfigurasi setelah perpindahan, jika menggunakan su alifpratama maka hanya berpindah ke pengguna tersebut tanpa mengubah lingkungan secara penuh, direktori kerja tetap di tempat sebelumnya dan variabel lingkungan seperti $PATH serta $HOME masih mengikuti pengguna sebelumnya, sedangkan jika menggunakan su - alifpratama maka perpindahan dilakukan secara penuh seperti simulasi login baru, direktori kerja akan berubah ke /home/alifpratama dan variabel lingkungan 
akan diperbarui sesuai dengan pengguna alifpratama.



2.  Prompt String (PS)

   a).Edit file .bash_profile, ganti prompt PS1 dengan ‘>’.

![Cuplikan layar 2025-03-25 231420](https://github.com/user-attachments/assets/f451d699-a54e-45f3-b9d6-0bd291469f61)

 b).Eksperimen hasil PS1

![Cuplikan layar 2025-03-25 231208](https://github.com/user-attachments/assets/ec061b44-6926-4878-883d-afb4aa44b681)

3. Log out

![image](https://github.com/user-attachments/assets/b03ebbad-ac3d-407a-baa5-402948b65eb9)

4. Bash script

    hasil jalankan script tersebut :
       -$ ./p1.sh ; ./p3.sh ; ./p2.sh

   ![image](https://github.com/user-attachments/assets/3d897be2-d75a-471e-956e-c180058623b1)

     -$ ./p1.sh &

   ![image](https://github.com/user-attachments/assets/89f9b233-926a-4bd5-bba1-33be977d1175)

       -$ ./p1.sh $ ./p2.sh & ./p3.sh &

   ![image](https://github.com/user-attachments/assets/3a2ed7b7-3c11-445d-84c8-a1256ef92047)

       -$ ( ./p1.sh ; ./p3.sh ) &

   ![image](https://github.com/user-attachments/assets/b31b1a19-6811-436f-accb-7ebc3dd9687a)

5. Jobs
 
 
   Hasil program yang dijalankan

       -$ jobs

   ![image](https://github.com/user-attachments/assets/4b7d27e8-ce6b-41f0-b6b5-527e81c25edf)


        -$ find / -print > files 2>/dev/null &

   ![image](https://github.com/user-attachments/assets/c77d45ad-7548-4ae6-8a99-8763e2f33bce)

       -$ jobs

    ![image](https://github.com/user-attachments/assets/273fa23f-94d0-489b-b771-efaf2470ae1b)



     Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke 
background

       -$ fg %1
   ![image](https://github.com/user-attachments/assets/75c0369c-080a-486f-aba9-088c14d3562e)

       -$ bg

   ![image](https://github.com/user-attachments/assets/9311acfe-0461-4d66-8df2-1ee479ca5646)



   Stop program background dengan utilitas kil

       -$ ps x

   ![image](https://github.com/user-attachments/assets/cea7ec99-6e45-4c0c-a47d-cd6f46d28bcb)

       -$ kill [Nomor PID] 

   ![image](https://github.com/user-attachments/assets/cb94ec50-fa76-40cf-a7c1-786c4f2eb226)

6. History

    a).Ganti nilai HISTSIZE dari 1000 menjadi 20

        -$ HISTSIZE=20

   ![image](https://github.com/user-attachments/assets/ecb8250f-42c9-4e66-945a-f1b5a7f968bd)

       -$ history

   ![image](https://github.com/user-attachments/assets/dbdb591a-3915-415a-8a6d-98affb17d0d4)

  b).Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir
     dilakukan
  
       -$ !-5
   
   ![image](https://github.com/user-attachments/assets/13188b6c-6190-47ac-8151-a66aee4add5b)

  c). Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer
      
       -$ !!
   
   ![image](https://github.com/user-attachments/assets/f219fbf1-17b4-4909-a05c-810d715b79e8)

   d).Ulangi instruksi pada history bufer nomor 150
   
       -$ !150
   
   ![image](https://github.com/user-attachments/assets/8a3867fb-98e6-4abf-a15a-f4d669ca030c)

   e).Ulangi instruksi dengan prefix “ls” 
   
       -$ !ls
  
   ![image](https://github.com/user-attachments/assets/8092bd82-7da0-4b18-889f-cfa48f62ead6)










   


















