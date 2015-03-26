#Itip - Tooltip jQuery plugin
Là một plugin gọn nhẹ  giúp bạn tạo ra tooltip đẹp một cách nhanh chóng với nhiều hiệu ứng đẹp từ [animate.css](http://daneden.github.io/animate.css/).

##Cách sử dụng: 

1.Download file về và copy 2 file Itip.css, jQuery.Itip.js vào thư mục thích hợp trong dự án của bạn.

2.Chèn hai file này vào file html bạn cần sử dụng tooltip, chú ý đường đẫn phải sửa lại cho phù hợp, phải đặt script của jQuery.Itip.js sau file thư viện jQuery, nếu bạn muốn có thêm nhiều hiệu ứng đẹp mắt cho tooltip hãy chèn thêm file animate.css (dowload bản mới nhất ở [đây](http://daneden.github.io/animate.css/)).
```html
	<head>
		<script type='text/javascript'src='jQuery.js'></script>

		<script type='text/javascript'src='jQuery.Itip.js'></script>
		<link rel="stylesheet" href="Itip.css" type="text/css" />
		<link rel="stylesheet" href="animate.css" type="text/css" />
	</head>
```

3.Kích hoạt tooltip.
```javascript
	<script>
		$(document).ready(function(){
			$('myElement').Itip();
		});
	</script>
```
  Như vậy bạn đã có một tooltip đơn giản nếu bạn muốn custom một số chức năng hãy tới bước 4.
4.Các tính năng của tooltip.
```javascript
 $('myElement').Itip(option);
```

Trong đó option có thể là đối tượng hoặc hàm cần thực thi.
* Các thuộc tính của option:
	* position: Xác định vị trí xuất hiện của Tooltip, gồm các giá trị left, right, top, bottom, LorR (tự động hiển thi bên trái hay phải dựa vào độ rộng của trình duyệt). Mặc định là 'top'.
	* content:   Chuỗi chứa nội dung của tooltip . Bạn có thể sủ dung data-Itip để truyền nội dung cho tooltip, nếu bạn sử dụng content nội dung của data-Itip sẽ được bỏ qua, bạn nên sử dụng content nếu nội dung bạn truyền vào tooltip có chứa các thẻ html. Mặc định content có giá trị là false.
	* autoClose: (true,false) tooltip sẽ tự động đóng khi mouseleaver hoặc khi click, mặc định là true.
	* triggerBy: ('hover' ,'click') Sự kiện kích hoạt tooltip.
	* animate:  (string) Chuỗi class cho hiệu ứng của animate.css mà bạn muốn sử dụng cho tooltip. Bạn có thể tìm ở đây
	* minWidth :  Độ dài tối đa của tooltip, vd: "100", "200".Mặc đinh là "100", đơn vị px.
	* maxWidth :  Độ dài tối thiểu của tooltip, vd: "100", "200".Mặc đinh là "150", đơn vị px.
	* AfterOpen: Hàm thực hiện sau khi tooltip xuất hiện.
	* AfterClose: Hàm thực hiện sau khi tooltip biến mất.
	* backGround: (string) Màu background của tooltip
	* color: (string) Màu chữ của tooltip
	* interaction: (true, false) Cho phép click hoăc hover lên tooltip. Măc định là false. 
* Các hàm có thể truyền vào option.
	* showItip: Kích hoạt tooltip xuất hiện.
	* hideItip: Kích hoạt ẩn tooltip.

[Một số demo về sử dụng Itip](http://thaitienblog.com/Itip_jQuery_plugin/demo.html#).




