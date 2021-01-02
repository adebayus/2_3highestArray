### This is a third-tier heading

You can use one `#` all the way up to `######` six for different heading sizes.
### Aplikasi Yang Digunakan

1. Vs Code

### Cara Menjalakan Aplikasi

2. node "nama_file.js"

### Sedikit Penjelasan Code

1. mendeklarasikan array 
```javascript
const data = [1,4,6,2,6,8,9,21,20, 14, 3,6,11,1,1,2,3,4,6,8,9,2,1,5,2,5,6,8,3,2]
```

2. membuat function untuk memilah nilai yang ganjil kemudian mereduce nilai yang sama dan mensorting dari tinggi ke besar
```javascript
function tigaTerbesar(data) {
    const ganjilReduceAndSort =  reduceValue(data)
    return ganjilReduceAndSort.forEach((x,index )=> { index <= 2 && console.log(`nilai Tertinggi ${index + 1} : ${x} `)   })
}

function reduceValue(ganjil){
    var tampungValue = [];
        
        // Loop through array values
        for(var value of ganjil){
            if(tampungValue.indexOf(value) === -1){
                tampungValue.push(value);
            }
        }
        tampungValue.sort(function(a, b) {
            return b - a;
          });

        return tampungValue;
}
```

3. memanggil fungsi yang sudah dibuat

```javascript
tigaTerbesar(data)
```