# <h1 align="center">Laporan Praktikum Modul 1 - ... </h1>
<p align="center">MUHAMMAD TETUKO KEMAL PASHA - 109082500181</p>

## Unguided 

### 1. [Soal]
#### soal1.go

```go
package main

import "fmt"

func main() {
	var (
		satu, dua, tiga string
		temp            string
	)
	fmt.Print("Masukan input string: ")
	fmt.Scanln(&satu)

	fmt.Print("Masukan input string: ")
	fmt.Scanln(&dua)

	fmt.Print("Masukan input string: ")
	fmt.Scanln(&tiga)

	fmt.Println("Output awal = ", satu, dua, tiga)
	temp = satu
	satu = dua
	dua = tiga
	tiga = temp
	fmt.Println("Output akhir = ", satu, dua, tiga)
}

```
### Output Unguided :

##### Output 
![Screenshot Output Unguided 1_1]https://github.com/tetukopasha-tech/109082500181_MUHAMMAD-TETUKO-KEMAL-PASHA/blob/main/modul1/output/Cuplikan%20layar%202026-03-14%20053938.png
[penjelasan] = PROGRAM INI MENJELASKAN MENYIMPAN VARIABEL SETIAP TEMPATNYA SAMA SEPERTI RETURN MATERI BARU 

### 2. [Soal]
#### soal2.go

```go
package main

import "fmt"

func main() {

	berhasil := true

	for i := 1; i <= 5; i++ {
		var g1, g2, g3, g4 string

		fmt.Printf("Percobaan %d: ", i)
		fmt.Scan(&g1, &g2, &g3, &g4)

		if g1 != "merah" || g2 != "kuning" || g3 != "hijau" || g4 != "ungu" {
			berhasil = false
		}
	}

	fmt.Printf("BERHASIL: %v\n", berhasil)
}


```
### Output Unguided :

##### Output 
![Screenshot Output Unguided 1_1]https://github.com/tetukopasha-tech/109082500181_MUHAMMAD-TETUKO-KEMAL-PASHA/blob/main/modul1/output/Cuplikan%20layar%202026-03-13%20010028.png
[penjelasan] = PROGRAM MENJELASKAN TENTANG PERULANGAN WARNA

### 3. [Soal]
#### soal3.go

```go
package main

import "fmt"

func main() {
	var beratGram int
	fmt.Print("Berat parsel (gram): ")
	fmt.Scan(&beratGram)

	kg := beratGram / 1000
	sisaGram := beratGram % 1000

	biayaKg := kg * 10000

	biayaTambahan := 0
	if kg < 10 {
		if sisaGram >= 500 {
			biayaTambahan = sisaGram * 5
		} else {
			biayaTambahan = sisaGram * 15
		}
	} else {
		biayaTambahan = 0
	}

	totalBiaya := biayaKg + biayaTambahan
	fmt.Printf("Detail berat: %d kg + %d gr\n", kg, sisaGram)
	fmt.Printf("Detail biaya: Rp. %d + Rp. %d\n", biayaKg, biayaTambahan)
	fmt.Printf("Total biaya: Rp. %d\n", totalBiaya)
}

```
### Output Unguided :

##### Output 
![Screenshot Output Unguided 1_1]https://github.com/tetukopasha-tech/109082500181_MUHAMMAD-TETUKO-KEMAL-PASHA/blob/main/modul1/output/Cuplikan%20layar%202026-03-14%20054358.png
[penjelasan] = MENJELASKAN PARSEL YANG SESUAI DENGAN DATANYA