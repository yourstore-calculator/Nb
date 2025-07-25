# Nb
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <title>حاسبة الأسعار</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      background-color: #f4f4f4;
      color: #333;
      direction: rtl;
      text-align: right;
      padding: 20px;
    }
    h1, h2 {
      text-align: center;
      margin-bottom: 10px;
    }
    .logo {
      text-align: center;
      margin-bottom: 10px;
    }
    .logo img {
      width: 140px;
    }
    .form-group {
      margin-bottom: 15px;
    }
    label {
      display: block;
      font-weight: bold;
    }
    input, select {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }
    button {
      background-color: #333;
      color: white;
      padding: 10px 15px;
      border: none;
      border-radius: 4px;
      margin-top: 10px;
      cursor: pointer;
    }
    button:hover {
      background-color: #444;
    }
    .result {
      background-color: #fff;
      padding: 15px;
      margin-top: 15px;
      border-radius: 5px;
      border: 1px solid #ddd;
    }
    .summary {
      margin-top: 25px;
      background-color: #e9f5ff;
      padding: 15px;
      border-radius: 8px;
      font-weight: bold;
      font-size: 18px;
    }
    .note {
      font-size: 14px;
      margin-top: 8px;
      color: #666;
    }
  </style>
</head>
<body>
  <div class="logo">
    <img src="https://i.imgur.com/ih5zjVj.png" alt="شعار الشركة" />
  </div>
  <h1>حاسبة الأسعار</h1>
  <div id="calculator">
    <!-- ستكمل هنا الحقول والأزرار -->    <div class="form-group">
      <label for="category">اختر القسم:</label>
      <select id="category">
        <option value="">-- اختر --</option>
        <option value="نوافذ">نوافذ</option>
        <option value="أبواب">أبواب</option>
        <option value="أبواب سحب">أبواب السحب</option>
      </select>
    </div>

    <div class="form-group">
      <label for="type">اختر النوع:</label>
      <select id="type"></select>
    </div>

    <div class="form-group" id="subTypeContainer" style="display:none;">
      <label for="subType">تفاصيل إضافية:</label>
      <select id="subType"></select>
    </div>

    <div class="form-group" id="curtainInput" style="display:none;">
      <label for="curtainSize">مقاس الستارة (الطول × العرض):</label>
      <input type="number" id="curtainLength" placeholder="الطول بالمتر">
      <input type="number" id="curtainWidth" placeholder="العرض بالمتر">
    </div>

    <div class="form-group" id="meshTypeContainer" style="display:none;">
      <label for="meshType">نوع الشبك:</label>
      <select id="meshType">
        <option value="">-- اختر --</option>
        <option value="ثابت">ثابت</option>
        <option value="سلايد">سلايد</option>
        <option value="فولدنج">فولدنج</option>
        <option value="باب">باب</option>
      </select>
    </div>

    <div class="form-group">
      <label for="height">الطول (بالمتر):</label>
      <input type="number" id="height" step="0.01" placeholder="مثال: 2.2">
    </div>

    <div class="form-group">
      <label for="width">العرض (بالمتر):</label>
      <input type="number" id="width" step="0.01" placeholder="مثال: 1">
    </div>

    <div class="form-group">
      <label for="quantity">الكمية:</label>
      <input type="number" id="quantity" value="1" min="1">
    </div>

    <button onclick="calculate()">📦 احسب</button>
    <button onclick="resetForm()">🔄 إعادة تعيين</button>
    <button onclick="saveAsWord()">💾 حفظ النتائج كـ Word</button>

    <div id="results"></div>
    <div id="summary" class="summary" style="display:none;"></div>
    <div class="note">🚚 الأسعار تشمل الشحن</div>
    <div class="note">💵 الأسعار لا تشمل التركيب</div>
  </div>

  <script>
    // هنا سيتم إدراج السكربت الخاص بالحسابات والأسعار
  </script>
</body>
</html>
