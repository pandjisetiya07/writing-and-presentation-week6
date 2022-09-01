# Minggu ke 6
## React Js Hooks
### Apa itu Hooks?
- yaitu memudahkan pengguna functional components agar bisa menggunakan state, dan lifecyle lainnya.
### Hooks 
- Hooks yg sering digunakan  adalah usState, dan useEffect dua hal ini sama dengan state, dan lifecycle di class yang biasa kita sering gunakan.
### Perbedaan functional component dengan class component
- seperti contoh di gambar ini:
![](slide%209,.png)

- Kedua component menghasilkan hal yg sama, namun class menggunakan state, dan functional menggunakan state hooks. namun untuk hasil SAMA.
### Kelebihan penggunaan hooks
- Dengan menggunakan functional component dan menggunakan hooks, maka code akan terlihat lebih pendek dan mudah dimengerti.
### Apa itu useState?
- useState adalah hooks pertama yang akan kita bahas, penggunaan useState sedikit berbeda dengan setState / state di class components, namun pengertian dari useState itu sendiri sama dengan state biasa.
### Cara penggunaan useState Hooks
1. Import useState dari react.
```
import { useState} from "react";
```
2. Menuliskan useState. hooks
```
const [nama, setNama] - useState("luthfi");
```
3. Pemanggilan Data.
```
<p> Halo, saya {nama} </p>
```
4. Update Status.
```
<button onClick={ setNama("david") }> ubah </button>
```

![](slide%2022,.png)

- Hasil dari code diatas.
![](slide%2023,.png)

### Update State
- State, bisa kita ubah menggunakan variable kedua dari state hooks, contoh jika kita memiliki kode seperti ini
```
const [nama, setNama] = useState("luthfi");
```
- maka kita tinggal menggunakan setNama() untuk mengupdatenya.
### Ubah state menggunakan onChange

![](slide%2026,.png)

- Hasil dari code diatas adalah:

![](slide%2027,.png)

### Array dalam useState Hooks
- kita bisa menggunakan array untuk menyimpan data dalam state. dengan memasukkan tanda [] dalam useState untuk menandakan bahwa state tsb merupakan array.
### Array dalam useState
 
![](slide%2030,.png)

- Hasil dari code diatas:

![](slide%2031,.png)


### Penggunaan useState hooks
- useState biasanya akan digunakan saat kamu menyimpan data suatu form yang nantinya akan di post ke api untuk di proses. selain itu kita bisa menyimpan data hasil get dari api tsb kedalam state menggunakan useState.

### Apa itu useEffect hooks?
- useEffect merupakan hooks yang bisa digunakan untuk menggunakan lifecycle pada functional component dengan mudah.
### Apa itu lifeCycle?
- lifeCycle yg ada pada hooks hanya menggunakan useEffect yg mengsatukan component DidMount, component DidUpdate, dan component WillUnmount.
### lifeCycle Structure

![](slide%2039,.png)

### Penggunaan useEffect
- Penggunaan useEffect bisa dimasukan sebelum melakukan render useEffect sendiri biasanya ditempatkan dibawah useState.
- Cara penggunaan useEffect
1. import useEffect
```
import {useEffect} from "react"
```
2. Tuliskan penggunaan useEffect hooks sebelum render
```
useEffect(() => {
    console.log("telah terjadi perubahan")
}, [nama])
```
- Full code di atas

![](slide%2044,.png)

- hasil yang di dapat dari code diatas adalah: setiap tombol ubah ditekan maka state nama akan berubah.

## Prop Types
- kita dapat mengirimkan sebuah data dalam bentuk (tipe data) apapun sebagai props. selain itu props types digunakan untuk menghindari bug pada saat pembuatan code.

### Pengertian Props Types 
- merupakan sebuah lib yang dapat membantu kamu untuk memeriksa data props yang km kirim agar sesuai dengan ekspektasi jika tidak sesai maka akan muncul pesan error.

### Cara penginstalan pada Props Types 
- ``` npm install prop-types ```

### Contoh penggunaan Props Types
```
import PropTypes from 'prop-types';
functional Header(props) {
    return (
        <> 
        <h2>Name: {props.char}</h2>
        <h2>Name: {props.age}</h2>
        </>
    )
}
Header.PropTypes = {
    char: PropTypes.string,
    age: PropTypes.number
}
```
- *Props yang akan dikirim harus sesuai dengan tipe data yang diinginkan.*

 ## React Router Dom
- React-router-dom adalah sebuah library yang dapat kita gunakan untuk membuat routing pada aplikasi React.js.
 
- Route adalah sebuah component yang mana akan menampilkan sebuah halaman apabila URL yang diberikan itu sesuai.
- React-router-dom bisa menerapkan server side rendering, apa sih yang di maksud dengan server side rendering? 
Yaitu tempat server mengembalikan halaman HTML yang siap dirender dan skrip JS yang diperlukan untuk membuat halaman menjadi interaktif . 

## React Redux
### pengertian dari Redux?
- library untuk mengelola dan memperbarui status aplikasi

- Terdapat beberapa konsep dasar redux diantaranya adalah:
1. store
2. action
3. dispatch

- Bentuk data yang dapat kita simpan di dalam redux-store adalah object.
- Tidak dapat memiliki lebih dari 1 redux store.
- cara agar kita dapat mengeksekusi sebuah redux action menggunakan dispatch.
- Untuk mengambil data dari redux store kita dapat menggunakan salah satu react-redux API yaitu useSelector.


