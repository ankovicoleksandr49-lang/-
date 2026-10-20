# -
<!DOCTYPE html>
<html lang="uk">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Бухгалтерія ВРУ | UKRAINE GTA 5 RP</title>
<style>
:root {
  --navy: #10264a;
  --blue: #1e477f;
  --bg: #f1f4f8;
  --white: #fff;
  --text: #1d2939;
  --muted: #667085;
  --border: #e1e7ef;
  --green: #14804a;
  --red: #c03939;
}
* { box-sizing: border-box; }
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: var(--bg);
  color: var(--text);
}
header {
  background: var(--navy);
  color: white;
  padding: 20px 28px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 15px;
  flex-wrap: wrap;
}
.brand { font-size: 21px; font-weight: bold; }
.brand small {
  display: block;
  font-size: 12px;
  color: #c7d5eb;
  margin-top: 6px;
  font-weight: normal;
}
.status {
  background: #233e64;
  border-radius: 8px;
  padding: 10px 14px;
  font-size: 13px;
}
.layout { display: flex; min-height: calc(100vh - 82px); }
aside {
  width: 230px;
  background: white;
  padding: 20px 12px;
  border-right: 1px solid var(--border);
  flex-shrink: 0;
}
.nav {
  display: block;
  width: 100%;
  text-align: left;
  border: 0;
  background: transparent;
  padding: 13px;
  margin-bottom: 5px;
  border-radius: 8px;
  color: #344054;
  cursor: pointer;
  font-size: 14px;
}
.nav:hover, .nav.active { background: #eaf0f9; color: var(--navy); font-weight: bold; }
main { padding: 28px; width: 100%; min-width: 0; }
h1 { font-size: 25px; margin: 0 0 8px; }
.subtitle { color: var(--muted); margin-bottom: 24px; font-size: 14px; }
.cards {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 15px;
  margin-bottom: 25px;
}
.card, .panel {
  background: white;
  border: 1px solid var(--border);
  border-radius: 12px;
  padding: 20px;
}
.card-label { font-size: 13px; color: var(--muted); }
.amount { font-size: 25px; font-weight: bold; margin-top: 13px; overflow-wrap: anywhere; }
.green { color: var(--green); }
.red { color: var(--red); }
.panel { margin-bottom: 20px; }
.panel h2 { font-size: 17px; margin: 0 0 18px; }
.toolbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 12px;
  margin-bottom: 16px;
}
button, input, select, textarea { font: inherit; }
.btn {
  background: var(--navy);
  color: white;
  border: 0;
  padding: 11px 15px;
  border-radius: 7px;
  cursor: pointer;
}
.btn:hover { background: var(--blue); }
.btn.secondary { background: #e9edf4; color: var(--navy); }
.btn.danger { background: #a92d35; }
table { width: 100%; border-collapse: collapse; font-size: 13px; }
th, td { padding: 13px 10px; border-bottom: 1px solid var(--border); text-align: left; }
th { color: var(--muted); background: #f8fafc; font-weight: 600; }
.table-wrap { overflow-x: auto; }
.tag { padding: 5px 8px; border-radius: 6px; font-size: 12px; background: #e9edf4; }
.tag.ok { color: var(--green); background: #e4f6ec; }
.tag.wait { color: #946200; background: #fff2cc; }
form { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 14px; }
.field { display: flex; flex-direction: column; gap: 7px; }
.field.full { grid-column: 1 / -1; }
label { font-size: 13px; font-weight: bold; }
input, select, textarea {
  border: 1px solid #cfd7e3;
  border-radius: 7px;
  padding: 11px;
  width: 100%;
  background: white;
}
textarea { min-height: 75px; resize: vertical; }
.actions { display: flex; gap: 8px; flex-wrap: wrap; }
.hidden { display: none !important; }
.notice {
  padding: 12px 14px;
  background: #fff5d9;
  border: 1px solid #f0dda0;
  border-radius: 8px;
  font-size: 13px;
  line-height: 1.5;
  margin-bottom: 20px;
}
footer { color: var(--muted); font-size: 12px; padding: 12px 0; }
@media(max-width: 950px) {
  .cards { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  aside { width: 185px; }
  main { padding: 18px; }
}
@media(max-width: 600px) {
  .layout { display: block; }
  aside { width: 100%; display: flex; overflow-x: auto; padding: 8px; }
  .nav { width: auto; min-width: max-content; }
  main { padding: 14px; }
  .cards { gap: 9px; }
  .card { padding: 13px; }
  .amount { font-size: 19px; }
  form { grid-template-columns: 1fr; }
  .field.full { grid-column: auto; }
}
</style>
</head>
<body>
<header>
  <div class="brand">
    БУХГАЛТЕРІЯ ВРУ
    <small>UKRAINE GTA 5 RP · Фінансове управління</small>
  </div>
  <div class="status">● Демо-режим · Локальні дані</div>
</header>

<div class="layout">
<aside>
  <button class="nav active" data-page="dashboard">▦ Огляд казни</button>
  <button class="nav" data-page="transactions">↕ Операції</button>
  <button class="nav" data-page="requests">▤ Заявки</button>
  <button class="nav" data-page="salaries">₴ Зарплати</button>
  <button class="nav" data-page="reports">▧ Звіти</button>
  <button class="nav" data-page="audit">◷ Журнал дій</button>
</aside>

<main>
  <div class="notice">
    <strong>Увага:</strong> це демонстраційна версія. Дані зберігаються
    у браузері цього пристрою. Авторизація Discord, спільна база,
    серверні права доступу та захист фінансових операцій ще не підключені.
    Не внось реальні паролі або конфіденційні дані.
  </div>

  <section id="dashboard" class="page">
    <h1>Огляд казни</h1>
    <div class="subtitle">Фінансовий стан Верховної Ради України</div>
    <div class="cards">
      <div class="card"><div class="card-label">Баланс казни</div><div class="amount" id="balance">0 ₴</div></div>
      <div class="card"><div class="card-label">Надходження</div><div class="amount green" id="income">0 ₴</div></div>
      <div class="card"><div class="card-label">Витрати</div><div class="amount red" id="expenses">0 ₴</div></div>
      <div class="card"><div class="card-label">Очікують розгляду</div><div class="amount" id="pending">0</div></div>
    </div>
    <div class="panel">
      <div class="toolbar">
        <h2>Останні фінансові операції</h2>
        <button class="btn" onclick="showPage('transactions')">Усі операції</button>
      </div>
      <div class="table-wrap"><table>
        <thead><tr><th>Дата</th><th>Тип</th><th>Призначення</th><th>Сума</th></tr></thead>
        <tbody id="recentRows"></tbody>
      </table></div>
    </div>
  </section>

  <section id="transactions" class="page hidden">
    <h1>Фінансові операції</h1>
    <div class="subtitle">Облік надходжень і витрат казни</div>
    <div class="panel">
      <h2>Додати операцію</h2>
      <form id="transactionForm">
        <div class="field"><label>Тип операції</label>
          <select id="txType"><option value="income">Надходження</option><option value="expense">Витрата</option></select>
        </div>
        <div class="field"><label>Сума (₴)</label><input id="txAmount" type="number" min="1" step="1" required></div>
        <div class="field"><label>Категорія</label>
          <select id="txCategory"><option>Фінансування</option><option>Зарплата</option><option>Обладнання</option><option>Адміністративні витрати</option><option>Інше</option></select>
        </div>
        <div class="field"><label>Дата</label><input id="txDate" type="date" required></div>
        <div class="field full"><label>Призначення платежу</label><textarea id="txDescription" required maxlength="300"></textarea></div>
        <div class="field full"><button class="btn">Зберегти операцію</button></div>
      </form>
    </div>
    <div class="panel"><h2>Історія операцій</h2><div class="table-wrap"><table>
      <thead><tr><th>Дата</th><th>Тип</th><th>Категорія</th><th>Призначення</th><th>Сума</th></tr></thead>
      <tbody id="txRows"></tbody>
    </table></div></div>
  </section>

  <section id="requests" class="page hidden">
    <h1>Заявки на фінансування</h1>
    <div class="subtitle">Реєстрація та розгляд заявок підрозділів</div>
    <div class="panel">
      <h2>Створити заявку</h2>
      <form id="requestForm">
        <div class="field"><label>Підрозділ</label><input id="reqDepartment" required maxlength="100"></div>
        <div class="field"><label>Сума (₴)</label><input id="reqAmount" type="number" min="1" required></div>
        <div class="field full"><label>Мета фінансування</label><textarea id="reqReason" required maxlength="300"></textarea></div>
        <div class="field full"><button class="btn">Подати заявку</button></div>
      </form>
    </div>
    <div class="panel"><h2>Реєстр заявок</h2><div class="table-wrap"><table>
      <thead><tr><th>Дата</th><th>Підрозділ</th><th>Мета</th><th>Сума</th><th>Статус</th><th>Дії</th></tr></thead>
      <tbody id="requestRows"></tbody>
    </table></div></div>
  </section>

  <section id="salaries" class="page hidden">
    <h1>Заробітні плати</h1>
    <div class="subtitle">Демонстраційний облік нарахувань працівникам</div>
    <div class="panel">
      <h2>Додати нарахування</h2>
      <form id="salaryForm">
        <div class="field"><label>ПІБ / RP-ім'я працівника</label><input id="salaryName" required maxlength="100"></div>
        <div class="field"><label>Посада</label><input id="salaryPosition" required maxlength="100"></div>
        <div class="field"><label>Сума (₴)</label><input id="salaryAmount" type="number" min="1" required></div>
        <div class="field"><label>Дата</label><input id="salaryDate" type="date" required></div>
        <div class="field full"><button class="btn">Додати нарахування</button></div>
      </form>
    </div>
    <div class="panel"><h2>Відомість зарплат</h2><div class="table-wrap"><table>
      <thead><tr><th>Дата</th><th>Працівник</th><th>Посада</th><th>Сума</th></tr></thead>
      <tbody id="salaryRows"></tbody>
    </table></div></div>
  </section>

  <section id="reports" class="page hidden">
    <h1>Фінансові звіти</h1>
    <div class="subtitle">Зведена інформація про рух коштів</div>
    <div class="panel">
      <h2>Підсумки за весь період</h2>
      <div class="cards">
        <div><div class="card-label">Початковий баланс</div><div class="amount" id="initialReport">0 ₴</div></div>
        <div><div class="card-label">Надходження</div><div class="amount green" id="incomeReport">0 ₴</div></div>
        <div><div class="card-label">Витрати</div><div class="amount red" id="expenseReport">0 ₴</div></div>
        <div><div class="card-label">Поточний баланс</div><div class="amount" id="balanceReport">0 ₴</div></div>
      </div>
      <button class="btn" onclick="exportCSV()">Експортувати операції в CSV</button>
    </div>
  </section>

  <section id="audit" class="page hidden">
    <h1>Журнал дій</h1>
    <div class="subtitle">Історія дій у цьому браузері</div>
    <div class="panel"><div class="table-wrap"><table>
      <thead><tr><th>Час</th><th>Подія</th></tr></thead>
      <tbody id="auditRows"></tbody>
    </table></div>
    <p class="subtitle">Цей журнал можна змінити через браузер. Для справжнього аудиту потрібне серверне зберігання.</p>
    </div>
  </section>
  <footer>Бухгалтерія ВРУ · UKRAINE GTA 5 RP · Демонстраційна версія</footer>
</main>
</div>

<script>
const KEY = "vru_accounting_demo_v1";
const initialState = {
  openingBalance: 1000000,
  transactions: [],
  requests: [],
  salaries: [],
  audit: []
};
let state;
try {
  state = JSON.parse(localStorage.getItem(KEY)) || structuredClone(initialState);
} catch {
  state = structuredClone(initialState);
}

function save() {
  localStorage.setItem(KEY, JSON.stringify(state));
}
function money(n) {
  return new Intl.NumberFormat("uk-UA", {
    style: "currency", currency: "UAH",
    maximumFractionDigits: 0
  }).format(n);
}
function safe(value) {
  return String(value ?? "").replace(/[&<>"']/g, c => ({
    "&":"&amp;", "<":"&lt;", ">":"&gt;",
    '"':"&quot;", "'":"&#39;"
  }[c]));
}
function log(message) {
  state.audit.unshift({ date: new Date().toLocaleString("uk-UA"), message });
  state.audit = state.audit.slice(0, 200);
}
function totals() {
  let income = 0, expenses = 0;
  state.transactions.forEach(t => {
    if (t.type === "income") income += t.amount;
    else expenses += t.amount;
  });
  return { income, expenses, balance: state.openingBalance + income - expenses };
}
function showPage(page) {
  document.querySelectorAll(".page").forEach(p => p.classList.add("hidden"));
  document.getElementById(page).classList.remove("hidden");
  document.querySelectorAll(".nav").forEach(b =>
    b.classList.toggle("active", b.dataset.page === page)
  );
  render();
}
document.querySelectorAll(".nav").forEach(b =>
  b.addEventListener("click", () => showPage(b.dataset.page))
);

function render() {
  const t = totals();
  document.getElementById("balance").textContent = money(t.balance);
  document.getElementById("income").textContent = money(t.income);
  document.getElementById("expenses").textContent = money(t.expenses);
  document.getElementById("pending").textContent =
    state.requests.filter(r => r.status === "Очікує").length;

  const txHTML = state.transactions.map(t => `
    <tr><td>${safe(t.date)}</td>
    <td><span class="tag ${t.type === "income" ? "ok" : ""}">${t.type === "income" ? "Надходження" : "Витрата"}</span></td>
    <td>${safe(t.category)}</td><td>${safe(t.description)}</td>
    <td class="${t.type === "income" ? "green" : "red"}">${t.type === "income" ? "+" : "−"}${money(t.amount)}</td></tr>
  `);
  document.getElementById("txRows").innerHTML = txHTML.join("") || emptyRow(5);
  document.getElementById("recentRows").innerHTML =
    state.transactions.slice(0, 5).map(t => `
      <tr><td>${safe(t.date)}</td><td>${t.type === "income" ? "Надходження" : "Витрата"}</td>
      <td>${safe(t.description)}</td><td>${money(t.amount)}</td></tr>
    `).join("") || emptyRow(4);

  document.getElementById("requestRows").innerHTML =
    state.requests.map(r => `<tr>
      <td>${safe(r.date)}</td><td>${safe(r.department)}</td>
      <td>${safe(r.reason)}</td><td>${money(r.amount)}</td>
      <td><span class="tag ${r.status === "Схвалено" ? "ok" : r.status === "Очікує" ? "wait" : ""}">${safe(r.status)}</span></td>
      <td>${r.status === "Очікує" ? `<div class="actions">
        <button class="btn" onclick="reviewRequest('${r.id}','Схвалено')">Схвалити</button>
        <button class="btn danger" onclick="reviewRequest('${r.id}','Відхилено')">Відхилити</button>
      </div>` : "—"}</td></tr>`).join("") || emptyRow(6);

  document.getElementById("salaryRows").innerHTML =
    state.salaries.map(s => `<tr><td>${safe(s.date)}</td>
      <td>${safe(s.name)}</td><td>${safe(s.position)}</td><td>${money(s.amount)}</td></tr>`
    ).join("") || emptyRow(4);

  document.getElementById("auditRows").innerHTML =
    state.audit.map(a => `<tr><td>${safe(a.date)}</td><td>${safe(a.message)}</td></tr>`
    ).join("") || emptyRow(2);

  document.getElementById("initialReport").textContent = money(state.openingBalance);
  document.getElementById("incomeReport").textContent = money(t.income);
  document.getElementById("expenseReport").textContent = money(t.expenses);
  document.getElementById("balanceReport").textContent = money(t.balance);
}
function emptyRow(n) {
  return `<tr><td colspan="${n}" style="color:#667085">Записів поки немає</td></tr>`;
}
function today() {
  const d = new Date();
  return `${d.getFullYear()}-${String(d.getMonth()+1).padStart(2,"0")}-${String(d.getDate()).padStart(2,"0")}`;
}
document.querySelectorAll('input[type="date"]').forEach(i => i.value = today());

document.getElementById("transactionForm").addEventListener("submit", e => {
  e.preventDefault();
  const type = document.getElementById("txType").value;
  const amount = Number(document.getElementById("txAmount").value);
  const description = document.getElementById("txDescription").value.trim();
  if (!Number.isSafeInteger(amount) || amount <= 0 || !description) return;
  if (type === "expense" && amount > totals().balance) {
    alert("Недостатньо коштів у казні!");
    return;
  }
  state.transactions.unshift({
    id: crypto.randomUUID(), type, amount,
    category: document.getElementById("txCategory").value,
    date: document.getElementById("txDate").value,
    description
  });
  log(`${type === "income" ? "Надходження" : "Витрата"}: ${description}, ${money(amount)}`);
  save(); e.target.reset();
  document.getElementById("txDate").value = today();
  render();
});

document.getElementById("requestForm").addEventListener("submit", e => {
  e.preventDefault();
  state.requests.unshift({
    id: crypto.randomUUID(),
    date: today(),
    department: document.getElementById("reqDepartment").value.trim(),
    amount: Number(document.getElementById("reqAmount").value),
    reason: document.getElementById("reqReason").value.trim(),
    status: "Очікує"
  });
  log("Створено заявку на фінансування");
  save(); e.target.reset(); render();
});
function reviewRequest(id, status) {
  const r = state.requests.find(x => x.id === id);
  if (!r || r.status !== "Очікує") return;
  if (status === "Схвалено") {
    if (r.amount > totals().balance) {
      alert("Недостатньо коштів у казні для схвалення заявки.");
      return;
    }
    // Схвалення заявки не проводить оплату автоматично.
  }
  r.status = status;
  log(`Заявка ${r.department}: ${status}`);
  save(); render();
}
document.getElementById("salaryForm").addEventListener("submit", e => {
  e.preventDefault();
  const amount = Number(document.getElementById("salaryAmount").value);
  if (!Number.isSafeInteger(amount) || amount <= 0) return;
  if (amount > totals().balance) {
    alert("Недостатньо коштів у казні!");
    return;
  }
  const salary = {
    date: document.getElementById("salaryDate").value,
    name: document.getElementById("salaryName").value.trim(),
    position: document.getElementById("salaryPosition").value.trim(),
    amount
  };
  state.salaries.unshift(salary);
  state.transactions.unshift({
    id: crypto.randomUUID(), type: "expense", amount,
    category: "Зарплата", date: salary.date,
    description: `Зарплата: ${salary.name} (${salary.position})`
  });
  log(`Нараховано зарплату: ${salary.name}, ${money(amount)}`);
  save(); e.target.reset();
  document.getElementById("salaryDate").value = today();
  render();
});
function exportCSV() {
  const rows = [["Дата","Тип","Категорія","Призначення","Сума"]];
  state.transactions.forEach(t => rows.push([
    t.date, t.type === "income" ? "Надходження" : "Витрата",
    t.category, t.description, t.amount
  ]));
  const csv = "\uFEFF" + rows.map(row =>
    row.map(cell => '"' + String(cell).replace(/"/g, '""') + '"').join(";")
  ).join("\r\n");
  const url = URL.createObjectURL(new Blob([csv], {type:"text/csv;charset=utf-8;"}));
  const a = document.createElement("a");
  a.href = url; a.download = "zvit_buhgalteriya_vru.csv"; a.click();
  URL.revokeObjectURL(url);
}
render();
</script>
</body>
</html>
