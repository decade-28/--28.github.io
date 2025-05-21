
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0" >
    <style>
        .container { padding: 20px; font-family: Arial; }
        .detail-link { color: blue; text-decoration: underline; }
    </style>
</head>
<body>
<div class="container">
    <h2>车辆信息查询结果</h2>
    <p>车牌号码：陕C 0289522</p>
    <p>车主：杜晓胜</p>
    <p>院系：计算机学院</p>
    <a href="#details" class="detail-link">查看详情</a>
    <div id="details" style="display:none; margin-top:20px;">
        <p>更多详细信息可联系学院办公室查询</p>
    </div>
</div>
<script>
    document.querySelector('.detail-link').addEventListener('click', function(e) {
        e.preventDefault();
        document.getElementById('details').style.display = 'block';
    });
</script>
</body>
</html>
