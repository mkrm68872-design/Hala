<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<title>غرفة الشات الأونلاين</title>

<!-- ربط مكتبة Supabase -->
<script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2.30.0/dist/supabase.min.js"></script>

<style>
body {
  font-family: Arial;
  background: #000;
  color: #fff;
  text-align: center;
  padding: 30px;
}

#messages {
  width: 90%;
  max-width: 500px;
  height: 300px;
  border: 2px solid #4caf50;
  margin: 20px auto;
  padding: 10px;
  overflow-y: auto;
  background: #111;
  text-align: right;
}

input, button {
  padding: 10px;
  margin: 5px;
  border-radius: 6px;
  border: none;
  font-size: 16px;
}

input {
  width: 300px;
}

button {
  background: #4caf50;
  color: white;
  cursor: pointer;
}
</style>
</head>

<body>

<h2>غرفة الشات السرية</h2>

<div id="messages">
  <div>👋 أهلاً بك في الشات</div>
</div>

<input id="msgInput" placeholder="اكتب رسالتك هنا">
<button onclick="sendMessage()">إرسال</button>

<script>
// ======= إعدادات Supabase =======
const SUPABASE_URL = "https://ioanzmertegakuswdkfv.supabase.co"; // ضع هنا URL المشروع
const SUPABASE_ANON_KEY = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6ImlvYW56bWVydGVnYWtla2F1c3dka2Z2Iiwicm9sZSI6ImFub24iLCJpYXQiOjE3Njg5MjE0MTMsImV4cCI6MjA4NDQ5NzQxM30.4jJ2AjzbWxOB6kzWMgCVcdY_lK-xZeEq5NAmnJWlYLI"; // ضع هنا الـ anon key

const supabase = supabase.createClient(SUPABASE_URL, SUPABASE_ANON_KEY);

// ======= إرسال الرسائل =======
async function sendMessage() {
  const msg = msgInput.value.trim();
  if (!msg) return;

  await supabase.from('messages').insert([{ text: msg }]);
  msgInput.value = "";
}

// ======= استقبال الرسائل لحظياً =======
supabase
  .channel('public:messages')
  .on('postgres_changes', { event: 'INSERT', schema: 'public', table: 'messages' }, payload => {
    const div = document.createElement("div");
    div.textContent = "💬 " + payload.new.text;
    messages.appendChild(div);
    messages.scrollTop = messages.scrollHeight;
  })
  .subscribe();
</script>

</body>
</html>
