# JavaScript-ile-Benzersiz-Liste-Alma

Bir dizi içerisinden benzersiz kayıt listesi alır.

Kullanımı
=================================

```
myLib = function(){
    function inArray(value, array){ return array.indexOf(value); }
    function getUniqueValue(input){
    	var output = [];
      for (var i = 0; i < input.length; i++)
      {
          if (inArray(input[i], output) == -1)
          {
              console.log("ÇIKTI: " + input[i]);
              output.push(input[i]);
          }
      }
      return output;
    }
    return{
        getList: getUniqueValue
    }
}();
```

Çalışan Örnek
=================================

https://jsfiddle.net/DeliPenguen/07uv0yvk/1/
