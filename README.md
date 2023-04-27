# TUGAS PRAKTIKUM BIG DATA
TI-3A 
Reynaldi Fakhri Pratama
18

## Chapter 4
Apache Spark SQL, Dataframes, dan Datasets

<table border="0">
 <tr>
    <td><b style="font-size:30px">Tugas pratikum</b></td>
 </tr>
 <tr>
    <td>
      <b style="font-size:15px">Menjalankan spark</b>
      <img src="/image/00_spark.png">
      <br>
      <hr>
      <b style="font-size:15px">Hasil spark running</b>
      <img src="/image/00_browser.png">
      <br>
      <hr>
      <b style="font-size:15px">1. dataframe</b>
      <br>
      <img src="/image/01_dataframe.png">
      <br>
      <hr>
      <b style="font-size:15px">2. dataframe mysql</b><br>
      <img src="/image/02_dataframe_mysql.png">
      <br>
      <hr>
      <b style="font-size:15px">3. convert df rdd</b><br>
      <img src="/image/03_convert_df_rdd.png">
      <br>
      <hr>
      <b style="font-size:15px">4. datasets</b><br>
      <img src="/image/04_datasets.png">
      <p style='font-size:10px'>error karena tidak menunjukkan adanya collumn bernama dept_location</p>
      <br>
      <hr>
      <b style="font-size:15px">5. convert df ds</b><br>
      <img src="/image/05_convert_df_ds.png">
      <hr>
      <b style="font-size:15px">6. access metadata</b><br>
      <img src="/image/06_access_metadata.png">
      <hr>
      <b style="font-size:15px">7. import text</b><br>
      <img src="/image/07_impor_txt.png">
      <hr>
      <b style="font-size:15px">8. import json</b><br>
      <img src="/image/08_impor_json.png">
      <hr>
      <b style="font-size:15px">9. import csv</b><br>
      <img src="/image/09_impor_csv.png">
      <hr>
   </td>
 </tr>
 <tr>
   <td colspan="2">
      <b>1. mylist dan myschema </b>
      <p >
         <b>mylist</b> => variabel yang digunakan dalam konteks mendefinisikan skema untuk DataFrame di PySpark. mylist biasanya berisi nama kolom.
         <br>
         <b>myschema</b> => mendefinisikan jenis data dan properti nullable dari setiap kolom.
      </p>
      <hr>
      <b>2. spark.createDataFrame </b>
      <p >
         <b>spark.createDataFrame()</b> => metode di PySpark yang digunakan untuk membuat DataFrame dari RDD yang ada, daftar atau DataFrame pandas yang sudah ada.
      </p>
      <hr>
      <b>3. parallelize, toDF </b>
      <p >
         <b>parallelize()</b> => metode yang digunakan di PySpark untuk mengubah daftar atau kumpulan data menjadi RDD.
         <br>
         <b>toDF()</b> => metode yang digunakan di PySpark untuk mengubah daftar atau kumpulan data menjadi DataFrame.
      </p>
      <hr>
      <b>4. hadoop, fs, put </b>
      <p>
         <b>hadoop</b> => alat baris perintah yang dapat digunakan untuk berinteraksi dengan Hadoop Distributed File System (HDFS).
         <br>
         <b>fs</b> => perintah untuk berinteraksi dengan HDFS.
         <br>
         <b>put</b> => subperintah yang digunakan untuk mengunggah file ke HDFS.
      </p>
      <hr>
      <b>5. pyspark.sql, SQLContext, createOrReplaceTempView, show </b>
      <p>
         <b>pyspark.sql</b> => modul di PySpark yang digunakan untuk memanipulasi dan meminta data di Spark SQL.
         <br>
         <b>SQLContext</b> => kelas yang digunakan untuk membuat konteks Spark SQL.
         <br>
         <b>createOrReplaceTempView()</b> => metode yang digunakan untuk membuat tampilan sementara dari DataFrame.
         <br>
         <b>show()</b> => metode yang digunakan untuk menampilkan isi DataFrame.
      </p>
      <hr>
      <b>6. textFile, map, lambda, strip, StructField, StringType </b>
      <p>
         <b>textFile()</b> => metode yang digunakan di PySpark untuk membaca file teks.
         <br>
         <b>map()</b> => metode yang digunakan di PySpark untuk mentransformasikan dan menyaring data.
         <br>
         <b>lambda()</b> => metode yang digunakan di PySpark untuk mentransformasikan dan menyaring data.
         <br>
         <b>strip()</b> => metode yang digunakan di PySpark untuk menghapus karakter spasi dari awal dan akhir string.
         <br>
         <b>StructField()</b> => kelas yang digunakan untuk mendefinisikan skema untuk DataFrame.
         <br>
         <b>StringType()</b> => kelas yang digunakan untuk mendefinisikan skema untuk DataFrame.
      </p>
      <hr>
      <b>7. spark.read.format(), jdbc(), options() dan load() </b>
      <p>
         <b>spark.read.format()</b> => metode yang digunakan di PySpark untuk membaca data dari file atau sumber data lainnya menjadi DataFrame.
         <br>
         <b>jdbc()</b> => metode yang digunakan di PySpark untuk membaca data dari database ke dalam DataFrame.
         <br>
         <b>options()</b> => metode yang digunakan di PySpark untuk mengatur opsi saat membaca atau menulis data.
         <br>
         <b>load()</b> => metode yang digunakan di PySpark untuk membaca data dari file ke dalam DataFrame.
      </p>
      <hr>
      <b>8. show()</b>
      <p>
         <b>show()</b> => metode yang digunakan di PySpark untuk menampilkan isi DataFrame.
      </p>
      <hr>
      <b>9. collect, rdd, take</b>
      <p>
         <b>collect()</b> => metode yang digunakan di PySpark untuk mengumpulkan data dari seluruh partisi menjadi satu daftar.
         <br>
         <b>rdd()</b> => metode yang digunakan di PySpark untuk mengubah DataFrame menjadi RDD.
         <br>
         <b>take()</b> => metode yang digunakan di PySpark untuk mengambil n baris pertama dari DataFrame.
      </p>
      <hr>
      <b> 10 makeRDD, Seq, createDataset</b>
      <p>
         <b>makeRDD()</b> => metode yang digunakan di PySpark untuk mengubah daftar atau kumpulan data menjadi RDD.
         <br>
         <b>Seq()</b> => metode yang digunakan di PySpark untuk mengubah daftar atau kumpulan data menjadi RDD.
         <br>
         <b>createDataset()</b> => metode yang digunakan di PySpark untuk membuat Dataset dari RDD yang ada, daftar atau Dataset pandas yang sudah ada.
      </p>
      <hr>
      <b>11. filter</b>
      <p>
         <b>filter()</b> => metode yang digunakan di PySpark untuk mentransformasikan dan menyaring data.
      </p>
      <hr>
      <b>12. as,toDF,first</b>
      <p>
         <b>as()</b> => metode yang digunakan di PySpark untuk mengubah nama kolom.
         <br>
         <b>toDF()</b> => metode yang digunakan di PySpark untuk mengubah daftar atau kumpulan data menjadi DataFrame.
         <br>
         <b>first()</b> => metode yang digunakan di PySpark untuk mengambil baris pertama dari DataFrame.
      </p>
      <hr>
      <b>13. listDatabases, listTables, listFunctions, isCached, select</b>
      <p>
         <b>listDatabases()</b> => metode yang digunakan di PySpark untuk menampilkan daftar database.
         <br>
         <b>listTables()</b> => metode yang digunakan di PySpark untuk menampilkan daftar tabel.
         <br>
         <b>listFunctions()</b> => metode yang digunakan di PySpark untuk menampilkan daftar fungsi.
         <br>
         <b>isCached()</b> => metode yang digunakan di PySpark untuk mengecek apakah DataFrame tersimpan di cache.
         <br>
         <b>select()</b> => metode yang digunakan di PySpark untuk memilih kolom yang akan ditampilkan.
      </p>
      <hr>
      <b>14. Read,text</b>
      <p>
         <b>Read()</b> => metode yang digunakan di PySpark untuk membaca data dari file atau sumber data lainnya menjadi DataFrame.
         <br>
         <b>text()</b> => metode yang digunakan di PySpark untuk membaca file teks.
      </p>
      <hr>
      <b>15. load,json,format,printSchema</b>
      <p>
         <b>load()</b> => metode yang digunakan di PySpark untuk membaca data dari file ke dalam DataFrame.
         <br>
         <b>json()</b> => metode yang digunakan di PySpark untuk membaca file JSON.
         <br>
         <b>format()</b> => metode yang digunakan di PySpark untuk membaca data dari file atau sumber data lainnya menjadi DataFrame.
         <br>
         <b>printSchema()</b> => metode yang digunakan di PySpark untuk menampilkan skema DataFrame.
      </p>
      <hr>
      <b>16. write,save</b>
      <p>
         <b>write()</b> => metode yang digunakan di PySpark untuk menyimpan data dari DataFrame ke file atau sumber data lainnya.
         <br>
         <b>save()</b> => metode yang digunakan di PySpark untuk menyimpan data dari DataFrame ke file.
      </p>
      <hr>
      <b>17. parquet</b>
      <p>
         <b>parquet()</b> => metode yang digunakan di PySpark untuk menyimpan data dari DataFrame ke file parquet.
      </p>
      <hr>
      <b>18. listDatabases, listTables, listFunctions, isCached, select</b>
      <p>
         <b>listDatabases()</b> => metode yang digunakan di PySpark untuk menampilkan daftar database.
         <br>
         <b>listTables()</b> => metode yang digunakan di PySpark untuk menampilkan daftar tabel.
         <br>
         <b>listFunctions()</b> => metode yang digunakan di PySpark untuk menampilkan daftar fungsi.
         <br>
         <b>isCached()</b> => metode yang digunakan di PySpark untuk mengecek apakah DataFrame tersimpan di cache.
         <br>
         <b>select()</b> => metode yang digunakan di PySpark untuk memilih kolom yang akan ditampilkan.
      </p>
   </td>
 </tr>

 
</table>
