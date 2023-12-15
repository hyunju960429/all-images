# 콘솔창 복붙 안될때
All pasting 이나 all pasting 치고 엔터




![image](https://github.com/hyunju960429/all-images/assets/145514544/8ee8f290-b0d8-4418-b1d7-9f4ac26e8841)


이미지파일이 안뜨거나 적게 뜰때 --> 새로고침
copy 
# 복사한 코드를 console창에 var har = 붙여넣기 + 엔터 (그 값은 객체이다)

# 객체가 har이라는 변수에 할당 되었고 그 아래에

# download.js 안에 내용을 복사하여 콘솔에 붙여넣으면 전체이미지 주소가 일괄적으로 나타난다

![image](https://github.com/hyunju960429/all-images/assets/145514544/567e2696-f963-471b-b698-15d42a268625)



그 다음 har() + 엔터

![image](https://github.com/hyunju960429/all-images/assets/145514544/49dfd46d-f32e-42bb-8975-caaacca60924)



```
var imageUrls = [];
har.log.entries.forEach(function (entry) {
  if (entry.response.content.mimeType.indexOf("image/") !== 0) return;
  imageUrls.push(entry.request.url);
});
console.log(imageUrls.join('\n'));
```
