# gitpreopor
{
 hn:"",
 patientName:"",
 operation:"",
 ward:"",
 date:"",
 checklist:{},
 assessment:{},
 education:[],
 recorder:""
}
<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<title>Pre-operative Visit</title>

<style>
body{
 font-family: Arial;
 padding:20px;
 background:#f5f7fa;
}

.card{
 background:white;
 padding:20px;
 border-radius:10px;
}

input,select,textarea{
 width:100%;
 padding:10px;
 margin:5px 0 15px;
}

button{
 background:#0066cc;
 color:white;
 padding:12px;
 border:none;
 border-radius:8px;
}

</style>

</head>

<body>


<h2>📝 บันทึกผู้ป่วยก่อนผ่าตัด (Pre-op Visit)</h2>


<div class="card">

<label>HN</label>
<input id="hn">


<label>ชื่อผู้ป่วย</label>
<input id="patientName">


<label>Ward</label>

<select id="ward">

<option>ศัลยกรรม</option>
<option>อายุรกรรม</option>
<option>พิเศษ</option>

</select>


<label>Diagnosis</label>
<textarea id="diagnosis"></textarea>


<label>Operation</label>
<textarea id="operation"></textarea>



<h3>Surgical Safety Checklist</h3>

<label>
<input type="checkbox" id="consent">
 Informed Consent
</label>

<br>

<label>
<input type="checkbox" id="idband">
 ID Band
</label>

<br>

<label>
<input type="checkbox" id="site">
 Surgical Site Marking
</label>


<h3>การเตรียมผู้ป่วย</h3>

<label>
<input type="checkbox">
 งดน้ำงดอาหาร
</label>

<br>

<label>
<input type="checkbox">
 ทำความสะอาดร่างกาย
</label>


<br><br>

<button onclick="savePreop()">
💾 บันทึก
</button>


</div>


<script src="visit.js"></script>

</body>
</html>git add index.html
