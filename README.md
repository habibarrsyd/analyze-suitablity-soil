<p align="center">
  <a href="https://github.com/habibarrsyd/tebet-house-price-clustering/">
    <img src="images/uji_tanah.jpg" alt="Uji Kelayakan Tanah" height="130">
  </a>
</p>

<p align="center">
  <img src="images/python_picture.png" alt="Py" height="60">
  <img src="images/collab_blom_png-removebg-preview.png" alt="Google Collab" height="80">
  <img src="images/vscode.png" alt="vscode-picture" height="60">

  </p>

<p align="center">
  Analisa Uji Kelayakan Tanah dengan menggunakan Decision Tree.
  <br></br>
  <em>Dataset by <a href="https://kaggle.com">Kaggle</a>.</em>
</p>

    
# Latar Belakang
<img src="images/tanah.jpeg" alt="Alt Text" height="150">


[Decision Tree for Analyze suitability soil](https://github.com/habibarrsyd/analyze-suitablity-soil)<br>
Kualitas tanah adalah faktor penting dalam mendukung keberhasilan pertanian, di mana aspek seperti drainase, bahan organik, kelembapan, dan pH tanah sangat memengaruhi kesuburan dan produktivitas. Pengelolaan yang buruk terhadap faktor-faktor ini dapat menurunkan kualitas tanah dan hasil panen. Dengan kemajuan teknologi, metode analisis seperti *decision tree* menjadi alat yang efektif untuk mengevaluasi kesesuaian tanah berdasarkan data. Pendekatan ini membantu petani memahami pola dan mengambil keputusan yang tepat untuk meningkatkan kualitas tanah, sehingga mendukung efisiensi dan keberlanjutan pertanian.
## Tools
[`^ kembali ke atas ^`](#)

### Software yang digunakan :
- Sistem Operasi: Linux Ubuntu/Windows/Mac OS
- Bahasa : Python Language Programming
- Text Editor : Google Collaboratory atau Visual Studio Code

## Proses :
### Baca Data
<img src="images/tanah.jpeg" alt="Alt Text" height="150">
### PREPROCESSING
#### Lihat Deskripsi Data
<img src="images/tanah.jpeg" alt="Alt Text" height="150">
#### Cek Kekosongan Data
<img src="images/tanah.jpeg" alt="Alt Text" height="150">
#### Encoding (Ubah Kategorikal jadi Numerikal)
<img src="images/tanah.jpeg" alt="Alt Text" height="150">
### Pisahkan Data Atribut dan Target
<img src="images/tanah.jpeg" alt="Alt Text" height="150">

### Analyze
#### Import dan Aplikasikan Model
<img src="images/tanah.jpeg" alt="Alt Text" height="150">
#### Visualisasikan Tree yang Terbentuk
<img src="images/tanah.jpeg" alt="Alt Text" height="150">
#### Evaluasi Metrik Pengujian
<img src="images/tanah.jpeg" alt="Alt Text" height="150">
#### Uji Data Baru


## Conclusion
Decision Tree bekerja dengan membagi data berdasarkan aturan hierarkis menggunakanfiturfitur tertentu. Pada node awal (root), fitur pertama yang digunakan adalah Drainage Quality. Jika nilai Drainage Quality <= 0.5, semua sampel langsung diklasifikasikan sebagai Not Suitable karena pada node ini entropy bernilai 0.0, yang berarti semua data di cabangtersebut termasuk dalam kelas yang sama. Namun, jika Drainage Quality > 0.5, keputusan dilanjutkanke node berikutnya menggunakan fitur pH Level. Pada tahap ini, jika pHLevel <=5.95, sampel juga diklasifikasikan sebagai Not Suitable (entropy = 0). Sebaliknya, jika pHLevel >5.95, data akan diperiksa lebih lanjut ke level berikutnya. Cabang lebih dalam melibatkan fitur Moisture Content (%). Jika Moisture Content (%) <=34.5, data langsung diklasifikasikan sebagai Not Suitable. Namun, jika nilai ini lebihbesar, model melanjutkan dengan memeriksa fitur Organic Matter (%). Keputusan akhir dibuat di leaf node, di mana setiap sampel diklasifikasikan berdasarkan mayoritas kelas pada datayangmencapai node tersebut. Misalnya, jika Organic Matter (%) <= 3.1, tanah dianggap Suitable, sedangkan jika nilainya lebih besar, tanah tetap diklasifikasikan sebagai Not Suitable. Prosesini memastikan bahwa setiap data baru dapat dipetakan ke dalam kategori yang sesuai secarasistematis.




