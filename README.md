# API_YANDEX
https://translate.yandex.net/api/v1.5/tr.json/translate?key=(API_KEY)&text=(sô muốn đổi)&lang=en-vi
### Ví Dụ 
`https://translate.yandex.net/api/v1.5/tr.json/translate?key=trnsl.1.1.20191108T164508Z.222adc669804138d.bef05749bd1a4f807cea2e17ca22fe3bb2b9713c&text=100000000000000&lang=en-vi`

**Output :**
>{"code":200,"lang":"en-vi","text":["Một trăm nghìn tỷ"]}

API_KEY lấy ở : https://translate.yandex.com/developers/keys

## CODE PHP
`<?php
$dataJ = json_decode(file_get_contents("https://translate.yandex.net/api/v1.5/tr.json/translate?key=trnsl.1.1.20191108T164508Z.222adc669804138d.bef05749bd1a4f807cea2e17ca22fe3bb2b9713c&text=$_GET[so]&lang=en-vi"));
echo $dataJ->text[0];
?>`

