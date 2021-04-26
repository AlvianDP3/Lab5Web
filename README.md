# Langkah-langkah Praktikum
Persiapan membuat dokumen HTML dengan nama file lab5_javascript.html seperti berikut.
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Mengenal JavaScript</title>
</head>
<body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
  <script>
      document.write("Hello World");
      console.log("Hello World");
  </script>
</body>
</html>

![latihan1](https://user-images.githubusercontent.com/56244029/116037849-dd1c7d80-a692-11eb-9105-e7f7b937f859.jpg)

# Javascrip Dasar
Pemakaian Alert sebagai property window.
```
<html>
<head>
<title>alert box</title>
</head>
<body>
<script language = "javascript">
<!--
 window.alert("ini merupakan pesan untuk anda");
//-->
</script>
</body>
</html>
```
Pemakaian method dalam objek
```
<html>
<head>
<title>skrip javascript</title>
</head>
<body>
percobaan memakai javascript:<br>
<script language = "javascript">
<!--
 document.write("selamat mencoba javascript<br>");
 document.write("semoga sukses!");
//-->
</script>
</body>
</html>
```
Pemakaian Prompt
```
<html>
<head>
<title>pemasukan data</title>
</head>
<body>
<script language = "javascript">
<!--
 var nama = prompt("siapa nama anda?","masukkan nama anda");
 document.write("hai, "+nama);
//-->
</script>
</body>
</html>
```
Pembuatan fungsi dan cara pemanggilannya
```
<html>
<head>
    <title>contoh program javascript</title>
    <script language="javascript">
    function pesan(){
        alert ("memanggil javascript lewat body onload")
        }
    </script>
</head>
<body onload=pesan()>
</body>
</html>
```
# Dasar Pemrograman Di Javascript
Operasi dasar aritmatika
```
<html>
<head>
    <title>contoh program javascript</title>

    <script language="javascript">
    function test(val1,val2)
    {
        document.write("<br>"+"perkalian : val1*val2 "+"<br>)
	document.write(val1*val2)
	document.write("<br>"+"pembagian : val1/val2 "+"<br>)
	document.write(val1/val2)
	document.write("<br>"+"penjumlahan : val1+val2 "+"<br>)
	document.write(val1+val2)
	document.write("<br>"+"pengurangan : val1-val2 "+"<br>)
	document.write(val1-val2)
	document.write("<br>"+"modulus : val1%val2 "+"<br>)
	document.write(val1%val2)
    }
    </script>
</head>
<body>
    <input type+"button" name="button1" value="arithmetic" onlick=test(9,4)>
</body>
</html>
```
Seleksi kondisi (if..else)
```
<html>
<head>
    <title>contoh if-else</title>
</head>
<body>
    <script language = "javascript">
    <!--
     var nilai = prompt("nilai (0-100): ", 0);
     var hasil = "";
     if (nilai >= 60)
     hasil = "lulus";
     else
     hasil = :"tidak lulus"l
     document.write("hasil: " + hasil);
    //-->
    </script>
</body>
</html>
```
Penggunaan operator switch untuk seleksi kondisi
```
<html>
<head>
    <title>contoh program javascript</title>

    <script language="javascript">
    function test()
    {
	val1=window.prompt("imput nilai (1-5):")
	switch
	{
	     case "1" :
	    	 document.write("bilangan satu")
	     	 break
	     case "2" :
	    	 document.write("bilangan dua")
	    	 break
	     case "3" :
	    	 document.write("bilangan tiga")
	    	 break
	     case "4" :
	    	 document.write("bilangan empat")
	    	 break
	     case "5" :
	    	 document.write("bilangan lima")
	    	 break
	     default :
	    	 document.write("bilangan lainnya")
	}
    }
     </script>
</head>
<body>
    <input type="button" name="button1" value="switch" onclick=test()>
</body>
</html>
```
# Pembuatan Form
Form Input
```
<html>
<head>
    <script language="javascript">
    function test () {
	var val1=document.kirim.TI.value
	if (val1%2==0)
	    document.kirim.T2.value="bilangan genap"
	else
	    document.kirim.T2.value"bilangan ganjil"
    }
    </script>
</head>
<body>
    <form method="POST" name="kirim">
	<p>BIL <input type="text" name="TI" size="20">
	MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
	<P><input type="button" value="TEBAK" name="B1" onclick=test()></p>
    </form>
</body>
</html>
```
Form Button.
```
<html>
<head>
    <title>objek document</title>
</head>
<body>
    <script language = "javascript">
    <!--
    function ubahWarnaLB(Warna) {
	document.bgColor = warna;
    }
    function ubahWarnaLD(warna) {
	document.fgColor = warna;
    }
  //-->
  </script>
  
  <h1>tes</h1>
  <form>
      <input type="button" value ="Latar Belakang Hijau" onClick="ubahWarnaLB('GREEN')">
      <input type="button" value ="Latar Belakang Putih" onClick="ubahWarnaLB('WHITE')">
      <input type="button" value ="Teks Kuning" onClick="ubahWarnaLD('YELLOW')">
      <input type="button" value ="Teks Biru" onClick="ubahWarnaLD('BLUE')">
  </form>
  <script language = "javascript">
  <!--
   document.write("Diamodifikasi teakhir pada " +
   document.lastModifiend);
  //-->
  </script>

</body>
</html>
```
# HTML DOM
Pilihan menggunakan checkBox dengan perhitungan otomatis
```
<!--
File: daftar menu.html
//-->
<html>
<head>
    <title>daftar</title>
    <script>
	function hitung(ele) {
	     var total = document.getElementById('total').value;
		 total = (total 7 parseInt(total) : 0);
	     var harga = 0;

	     if (ele.checked) {
		 harga = ele.value;
		 total = perseInt(harga);
	     } else {
		 harga = ele.value;
		 if (total >0);
		     total -= perseInt(harga);
	     }
	     document.getElementById('Total').value = total;
	}
     </script>
</head>
<body>
     <h1>Daftar Menu Makanan</h1>
     <Label><input type="checkbox" value="5000" id="menu1" onlick="hitung(this);" /> Ayam Goreng Rp. 5000</label><br />
     <Label><input type="checkbox" value="500" id="menu1" onlick="hitung(this);" /> Tempe Goreng Rp. 500</label><br />
     <Label><input type="checkbox" value="2500" id="menu1" onlick="hitung(this);" /> Telur Dadar Rp. 2500</label><br />
     <strong>Total Bayar: Rp. <input id="total" type"text" /></strong>
</body>
</html>
```
# Pertanyaan dan Tugas
1. Buat script untuk melakukan validasi pada isian form.
```
<!DOCTYPE HTML>  
<html>
<head>
<style>
.error {color: #FF0000;}
</style>
</head>
<body>  

<?php
// define variables and set to empty values
$nameErr = $emailErr = $genderErr = $websiteErr = "";
$name = $email = $gender = $comment = $website = "";

if ($_SERVER["REQUEST_METHOD"] == "POST") {
  if (empty($_POST["name"])) {
    $nameErr = "Name is required";
  } else {
    $name = test_input($_POST["name"]);
    // check if name only contains letters and whitespace
    if (!preg_match("/^[a-zA-Z ]*$/",$name)) {
      $nameErr = "Only letters and white space allowed"; 
    }
  }
  
  if (empty($_POST["email"])) {
    $emailErr = "Email is required";
  } else {
    $email = test_input($_POST["email"]);
    // check if e-mail address is well-formed
    if (!filter_var($email, FILTER_VALIDATE_EMAIL)) {
      $emailErr = "Invalid email format"; 
    }
  }
    
  if (empty($_POST["website"])) {
    $website = "";
  } else {
    $website = test_input($_POST["website"]);
    // check if URL address syntax is valid (this regular expression also allows dashes in the URL)
    if (!preg_match("/\b(?:(?:https?|ftp):\/\/|www\.)[-a-z0-9+&@#\/%?=~_|!:,.;]*[-a-z0-9+&@#\/%=~_|]/i",$website)) {
      $websiteErr = "Invalid URL"; 
    }
  }

  if (empty($_POST["comment"])) {
    $comment = "";
  } else {
    $comment = test_input($_POST["comment"]);
  }

  if (empty($_POST["gender"])) {
    $genderErr = "Gender is required";
  } else {
    $gender = test_input($_POST["gender"]);
  }
}

function test_input($data) {
  $data = trim($data);
  $data = stripslashes($data);
  $data = htmlspecialchars($data);
  return $data;
}
?>

<h2>PHP Form Validation Example</h2>
<p><span class="error">* required field.</span></p>
<form method="post" action="<?php echo htmlspecialchars($_SERVER["PHP_SELF"]);?>">  
  Name: <input type="text" name="name" value="<?php echo $name;?>">
  <span class="error">* <?php echo $nameErr;?></span>
  <br><br>
  E-mail: <input type="text" name="email" value="<?php echo $email;?>">
  <span class="error">* <?php echo $emailErr;?></span>
  <br><br>
  Website: <input type="text" name="website" value="<?php echo $website;?>">
  <span class="error"><?php echo $websiteErr;?></span>
  <br><br>
  Comment: <textarea name="comment" rows="5" cols="40"><?php echo $comment;?></textarea>
  <br><br>
  Gender:
  <input type="radio" name="gender" <?php if (isset($gender) && $gender=="female") echo "checked";?> value="female">Female
  <input type="radio" name="gender" <?php if (isset($gender) && $gender=="male") echo "checked";?> value="male">Male
  <span class="error">* <?php echo $genderErr;?></span>
  <br><br>
  <input type="submit" name="submit" value="Submit">  
</form>

<?php
echo "<h2>Your Input:</h2>";
echo $alvian;
echo "<br>";
echo $alviandwipramono12@gmail.com;
echo "<br>";
echo $website;
echo "<br>";
echo $comment;
echo "<br>";
echo $gender;
?>

</body>
</html>
```

![image](https://user-images.githubusercontent.com/56244029/116038605-db06ee80-a693-11eb-90bf-8d71300a03ec.png)
