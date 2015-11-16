For IOH

##### 1. 需把PPT匯出成PNG檔，並把所有圖檔放在同一個資料夾裡後丟到slides資料夾內
##### 2. 視情況修改 *index.html* 中的 *var dir* (路徑)
```sh
	$(document).ready(function(){
	var dir = "slides/test/";
	var fileextension = ".PNG";`
```
##### 3. 視情況修改 *js/jquery.presentation-full.js*  的  *fileName* 中 */test/* 
```sh
	 dataType: 'html',
         type: 'POST',
         data: { timeContent: timeContent, fileName: "slides/test/timeStamp.txt"},
         error: function(){
         	alert("fail");
         }
```

##### 4.每次按下一頁時會把時間記錄下來，並存成 *timeStamp.txt*，目前的路徑是在 *slides/test/* 裡
##### 5.DEMO 
http://140.116.247.27/slideShow/