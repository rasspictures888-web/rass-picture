<!DOCTYPE html>
<html lang="am">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RAS Pictures - Dashboard</title>
    <style>
        :root {
            --primary-color: #1a1a1a;
            --accent-color: #cca43b;
            --bg-color: #f4f6f9;
            --card-bg: #ffffff;
            --text-color: #333;
            --success-color: #2ec4b6;
            --danger-color: #e71d36;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
        }

        .container {
            width: 100%;
            max-width: 600px;
            padding: 20px;
            box-sizing: border-box;
        }

        header {
            text-align: center;
            margin-bottom: 25px;
            padding: 20px;
            background: var(--primary-color);
            color: #fff;
            border-radius: 15px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }

        header h1 {
            margin: 10px 0 5px 0;
            font-size: 24px;
            letter-spacing: 1px;
            color: var(--accent-color);
        }

        .auth-bar {
            background: var(--card-bg);
            padding: 15px;
            border-radius: 12px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            margin-bottom: 20px;
            text-align: center;
        }

        .auth-bar p {
            margin: 0 0 10px 0;
            font-size: 13px;
            color: #666;
        }

        .btn-google {
            background: #4285F4;
            color: #fff;
            border: none;
            padding: 10px 20px;
            border-radius: 8px;
            font-size: 14px;
            font-weight: bold;
            cursor: pointer;
        }

        .btn-google:hover { background: #3367d6; }

        .btn-signout {
            background: #eee;
            color: #333;
            border: none;
            padding: 6px 14px;
            border-radius: 6px;
            font-size: 12px;
            cursor: pointer;
            margin-left: 10px;
        }

        .signed-in-badge {
            display: inline-flex;
            align-items: center;
            font-size: 13px;
            color: var(--success-color);
            font-weight: bold;
        }

        .dashboard-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
            margin-bottom: 25px;
        }

        .card {
            background: var(--card-bg);
            padding: 15px;
            border-radius: 12px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            text-align: center;
            border-top: 4px solid var(--accent-color);
        }

        .card.full-width {
            grid-column: span 2;
            border-top-color: var(--primary-color);
        }

        .card h3 {
            margin: 0 0 8px 0;
            font-size: 14px;
            color: #777;
            text-transform: uppercase;
        }

        .card .value {
            font-size: 20px;
            font-weight: bold;
            color: var(--primary-color);
        }

        .form-section {
            background: var(--card-bg);
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.05);
            margin-bottom: 25px;
        }

        .form-section h2 {
            margin-top: 0;
            font-size: 18px;
            border-bottom: 2px solid #eee;
            padding-bottom: 10px;
            color: var(--primary-color);
        }

        .input-group {
            margin-bottom: 15px;
        }

        .input-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: 600;
            font-size: 14px;
        }

        .input-group input, .input-group select {
            width: 100%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 8px;
            box-sizing: border-box;
            font-size: 16px;
        }

        .btn-submit {
            width: 100%;
            background: var(--primary-color);
            color: #fff;
            border: none;
            padding: 12px;
            border-radius: 8px;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            transition: background 0.3s;
        }

        .btn-submit:hover { background: #333; }
        .btn-submit:disabled { opacity: 0.6; cursor: not-allowed; }

        .history-section {
            background: var(--card-bg);
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.05);
        }

        .history-section h2 {
            margin-top: 0;
            font-size: 18px;
            border-bottom: 2px solid #eee;
            padding-bottom: 10px;
            color: var(--primary-color);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .clear-btn {
            background: var(--danger-color);
            color: white;
            border: none;
            padding: 5px 10px;
            border-radius: 5px;
            font-size: 12px;
            cursor: pointer;
        }

        .transaction-list {
            list-style: none;
            padding: 0;
            margin: 0;
            max-height: 400px;
            overflow-y: auto;
        }

        .transaction-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 12px 10px;
            border-bottom: 1px solid #eee;
            font-size: 14px;
        }

        .transaction-item:last-child { border-bottom: none; }

        .txn-details { display: flex; flex-direction: column; }
        .txn-date { font-size: 11px; color: #888; }
        .txn-people { font-size: 12px; color: #555; margin-top: 2px; }
        .txn-amount { font-weight: bold; }

        .income-cash { color: var(--success-color); }
        .income-trans { color: #0077b6; }
        .expense { color: var(--danger-color); }

        .empty-state, .loading-state {
            text-align: center;
            color: #999;
            padding: 20px;
            font-size: 14px;
        }

        #app-content { display: none; }

        #sync-status {
            text-align: center;
            font-size: 11px;
            color: #999;
            margin-top: 10px;
        }

        /* Login screen */
        #login-screen {
            max-width: 340px;
            margin: 80px auto 0 auto;
            background: var(--card-bg);
            padding: 30px 25px;
            border-radius: 15px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            text-align: center;
        }
        #login-screen h2 { margin-top: 0; color: var(--primary-color); }
        #login-screen input {
            width: 100%;
            box-sizing: border-box;
            padding: 12px;
            margin: 15px 0;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 15px;
            text-align: center;
        }
        #login-screen button {
            width: 100%;
            padding: 12px;
            background: var(--primary-color);
            color: var(--accent-color);
            border: none;
            border-radius: 8px;
            font-size: 15px;
            font-weight: bold;
            cursor: pointer;
        }
        #login-error { color: var(--danger-color); font-size: 13px; min-height: 18px; margin: 0; }
        #logout-bar {
            text-align: right;
            margin-bottom: 10px;
        }
        #logout-bar button {
            background: #eee;
            color: #333;
            border: none;
            padding: 6px 14px;
            border-radius: 6px;
            font-size: 12px;
            cursor: pointer;
        }
        #setup-banner {
            display: none;
            background: #fff8e1;
            border: 1px solid #cca43b;
            border-radius: 10px;
            padding: 14px;
            font-size: 12px;
            margin-bottom: 15px;
            word-break: break-all;
        }
    </style>
</head>
<body>

<div class="container">
    <header>
        <h1>RAS PICTURES</h1>
        <p style="margin: 0; font-size: 12px; color: #aaa;">የዕለት የሂሳብ መቆጣጠሪያ</p>
    </header>

    <div id="login-screen">
        <h2>🔒 መግቢያ</h2>
        <p style="font-size:13px;color:#888;">የይለፍ ቃል ያስገቡ</p>
        <input type="password" id="password-input" placeholder="የይለፍ ቃል" autocomplete="off">
        <p id="login-error"></p>
        <button id="login-btn">ግባ</button>
    </div>

    <div id="app-content">
        <div id="logout-bar" style="display:none;">
            <button id="logout-btn">ውጣ</button>
        </div>
        <div id="setup-banner"></div>
        <div class="dashboard-grid">
            <div class="card">
                <h3>የካሽ ገቢ (Cash)</h3>
                <div id="total-cash" class="value">0.00 ብር</div>
            </div>
            <div class="card">
                <h3>የትራንዛክሽን ገቢ</h3>
                <div id="total-trans" class="value">0.00 ብር</div>
            </div>
            <div class="card">
                <h3>አጠቃላይ ወጪ</h3>
                <div id="total-expense" class="value">0.00 ብር</div>
            </div>
            <div class="card">
                <h3>የተነሱ ሰዎች</h3>
                <div id="total-people" class="value">0 ሰው</div>
            </div>
            <div class="card full-width">
                <h3>ጠቅላላ ቀሪ ሂሳብ (Net Balance)</h3>
                <div id="net-balance" class="value" style="color: var(--accent-color); font-size: 24px;">0.00 ብር</div>
            </div>
        </div>

        <div class="form-section">
            <h2>አዲስ መረጃ መመዝገቢያ</h2>
            <form id="accounting-form">
                <div class="input-group">
                    <label for="type">የመረጃው አይነት</label>
                    <select id="type" required>
                        <option value="cash">ገቢ - በካሽ (Cash)</option>
                        <option value="transaction">ገቢ - በትራንዛክሽን (CBE Birr / Telebirr)</option>
                        <option value="expense">ወጪ (Expense)</option>
                    </select>
                </div>

                <div class="input-group">
                    <label for="amount">የገንዘብ መጠን (በብር)</label>
                    <input type="number" id="amount" placeholder="ምሳሌ፡ 200" required min="0" step="0.01">
                </div>

                <div class="input-group" id="people-group">
                    <label for="people">የተነሱ ሰዎች ቁጥር (ለገቢ ብቻ)</label>
                    <input type="number" id="people" placeholder="ምሳሌ፡ 2" value="0" min="0">
                </div>

                <div class="input-group">
                    <label for="description">ማብራሪያ / ስም</label>
                    <input type="text" id="description" placeholder="ምሳሌ፡ የፎቶ ቀረጻ ወይም የቤት ኪራይ" required>
                </div>

                <button type="submit" class="btn-submit" id="submit-btn">መዝግብ</button>
            </form>
        </div>

        <div class="history-section">
            <h2>
                የግብይት ታሪክ (Transactions)
                <button class="clear-btn" onclick="clearData()">ሁሉንም አጥፋ</button>
            </h2>
            <ul id="transaction-list" class="transaction-list">
                <li class="loading-state">በመጫን ላይ...</li>
            </ul>
            <p id="sync-status"></p>
        </div>
    </div>
</div>

<script>
    // ==== CONFIG ====
    // 1) Set your own password here (anyone who knows this can log in):
    const PASSWORD = 'ras2024';

    // 2) Cloud storage (JSONBin.io - free, no Google account needed).
    //    Get a free "X-Master-Key" at https://jsonbin.io (sign up, then Dashboard > API Keys)
    //    Paste it below. Leave JSONBIN_BIN_ID empty the very first time you run the app -
    //    it will create the shared storage automatically and show you an ID to paste back in here.
    const JSONBIN_API_KEY = '$2a$10$lMLUzAaMUjaYhSHfVXPrPuv3SGLpp6/0sEiTD1F95vWXLWAKbMHee';   // <-- paste your X-Master-Key here
    let   JSONBIN_BIN_ID  = '';   // <-- after first run, paste the generated Bin ID here

    let transactions = [];

    // ==== LOGIN ====
    window.addEventListener('load', () => {
        if (localStorage.getItem('ras_logged_in') === 'true') {
            enterApp();
        }
        document.getElementById('login-btn').addEventListener('click', tryLogin);
        document.getElementById('password-input').addEventListener('keydown', (e) => {
            if (e.key === 'Enter') tryLogin();
        });
        document.getElementById('logout-btn').addEventListener('click', logout);
    });

    function tryLogin() {
        const val = document.getElementById('password-input').value;
        if (val === PASSWORD) {
            localStorage.setItem('ras_logged_in', 'true');
            enterApp();
        } else {
            document.getElementById('login-error').innerText = 'የተሳሳተ የይለፍ ቃል';
        }
    }

    function logout() {
        localStorage.removeItem('ras_logged_in');
        document.getElementById('login-screen').style.display = 'block';
        document.getElementById('app-content').style.display = 'none';
        document.getElementById('password-input').value = '';
    }

    async function enterApp() {
        document.getElementById('login-screen').style.display = 'none';
        document.getElementById('app-content').style.display = 'block';
        document.getElementById('logout-bar').style.display = 'block';
        await loadData();
    }

    // ==== JSONBIN HELPERS ====
    async function jsonbinCreate() {
        const res = await fetch('https://api.jsonbin.io/v3/b', {
            method: 'POST',
            headers: {
                'Content-Type': 'application/json',
                'X-Master-Key': JSONBIN_API_KEY,
                'X-Bin-Name': 'ras_pictures_transactions'
            },
            body: JSON.stringify([])
        });
        if (!res.ok) throw new Error('Create failed: ' + res.status);
        const data = await res.json();
        return data.metadata.id;
    }

    async function jsonbinRead(id) {
        const res = await fetch(`https://api.jsonbin.io/v3/b/${id}/latest`, {
            headers: { 'X-Master-Key': JSONBIN_API_KEY }
        });
        if (!res.ok) throw new Error('Read failed: ' + res.status);
        const data = await res.json();
        return data.record;
    }

    async function jsonbinUpdate(id, record) {
        const res = await fetch(`https://api.jsonbin.io/v3/b/${id}`, {
            method: 'PUT',
            headers: {
                'Content-Type': 'application/json',
                'X-Master-Key': JSONBIN_API_KEY
            },
            body: JSON.stringify(record)
        });
        if (!res.ok) throw new Error('Update failed: ' + res.status);
    }

    // ==== DATA LOAD / SAVE ====
    async function loadData() {
        const banner = document.getElementById('setup-banner');

        if (!JSONBIN_API_KEY) {
            banner.style.display = 'block';
            banner.innerHTML = '⚠ ማከማቻ ገና አልተዋቀረም። ነጻ የ API ቁልፍ ከ <a href="https://jsonbin.io" target="_blank">jsonbin.io</a> ውሰድ እና በኮዱ ውስጥ JSONBIN_API_KEY ላይ ለጥፍ።';
            transactions = [];
            render();
            return;
        }

        if (!JSONBIN_BIN_ID) {
            setSyncStatus('የመጀመሪያ ጊዜ ማዋቀር በመካሄድ ላይ...');
            try {
                JSONBIN_BIN_ID = await jsonbinCreate();
                banner.style.display = 'block';
                banner.innerHTML = '✅ ማከማቻ ተፈጥሯል! ይህን ID ኮፒ አድርገህ በኮዱ ውስጥ JSONBIN_BIN_ID ላይ ለጥፍ ከዚያም እንደገና ወደ GitHub ስቀል፦<br><b>' + JSONBIN_BIN_ID + '</b>';
                transactions = [];
                setSyncStatus('✓ ተዘጋጅቷል (ID ን አስቀምጥ)');
            } catch (error) {
                console.error('Setup error:', error);
                setSyncStatus('⚠ ማዋቀር አልተቻለም');
                transactions = [];
            }
            render();
            return;
        }

        setSyncStatus('በመጫን ላይ...');
        try {
            transactions = await jsonbinRead(JSONBIN_BIN_ID);
            if (!Array.isArray(transactions)) transactions = [];
            setSyncStatus('✓ ተመሳስሏል');
        } catch (error) {
            console.error('Load error:', error);
            transactions = [];
            setSyncStatus('⚠ መጫን አልተቻለም');
        }
        render();
    }

    async function saveAndRender() {
        submitBtn.disabled = true;
        submitBtn.innerText = 'በመላክ ላይ...';
        setSyncStatus('በማስቀመጥ ላይ...');
        try {
            if (JSONBIN_API_KEY && JSONBIN_BIN_ID) {
                await jsonbinUpdate(JSONBIN_BIN_ID, transactions);
                setSyncStatus('✓ ተቀምጧል');
            } else {
                setSyncStatus('⚠ ማከማቻ አልተዋቀረም - ውሂብ አልተቀመጠም');
            }
        } catch (error) {
            console.error('Save error:', error);
            setSyncStatus('⚠ ማስቀመጥ አልተቻለም');
        }
        submitBtn.disabled = false;
        submitBtn.innerText = 'መዝግብ';
        render();
    }

    function setSyncStatus(msg) {
        const el = document.getElementById('sync-status');
        if (el) el.innerText = msg;
    }

    // ==== FORM / RENDER ====
    const form = document.getElementById('accounting-form');
    const typeInput = document.getElementById('type');
    const amountInput = document.getElementById('amount');
    const peopleInput = document.getElementById('people');
    const descriptionInput = document.getElementById('description');
    const peopleGroup = document.getElementById('people-group');
    const submitBtn = document.getElementById('submit-btn');

    typeInput.addEventListener('change', () => {
        if (typeInput.value === 'expense') {
            peopleGroup.style.display = 'none';
            peopleInput.value = '0';
        } else {
            peopleGroup.style.display = 'block';
        }
    });

    form.addEventListener('submit', async (e) => {
        e.preventDefault();

        const transaction = {
            id: Date.now(),
            type: typeInput.value,
            amount: parseFloat(amountInput.value),
            people: parseInt(peopleInput.value) || 0,
            description: descriptionInput.value,
            date: new Date().toLocaleDateString('am-ET', {hour: '2-digit', minute:'2-digit'})
        };

        transactions.unshift(transaction);
        await saveAndRender();
        form.reset();
        peopleGroup.style.display = 'block';
    });

    function render() {
        const list = document.getElementById('transaction-list');
        list.innerHTML = '';

        let totalCash = 0, totalTrans = 0, totalExpense = 0, totalPeople = 0;

        if (transactions.length === 0) {
            list.innerHTML = '<li class="empty-state">እስካሁን የተመዘገበ ግብይት የለም</li>';
        }

        transactions.forEach(txn => {
            if (txn.type === 'cash') {
                totalCash += txn.amount;
                totalPeople += txn.people;
            } else if (txn.type === 'transaction') {
                totalTrans += txn.amount;
                totalPeople += txn.people;
            } else if (txn.type === 'expense') {
                totalExpense += txn.amount;
            }

            const li = document.createElement('li');
            li.className = 'transaction-item';

            let typeClass = '', typeLabel = '', amountSign = '+';
            if (txn.type === 'cash') { typeClass = 'income-cash'; typeLabel = 'ካሽ'; }
            else if (txn.type === 'transaction') { typeClass = 'income-trans'; typeLabel = 'ትራንዛክሽን'; }
            else { typeClass = 'expense'; typeLabel = 'ወጪ'; amountSign = '-'; }

            li.innerHTML = `
                <div class="txn-details">
                    <strong>${escapeHtml(txn.description)} (${typeLabel})</strong>
                    <span class="txn-date">${txn.date}</span>
                    ${txn.people > 0 ? `<span class="txn-people">👥 የተነሱ ሰዎች፡ ${txn.people}</span>` : ''}
                </div>
                <div class="txn-amount ${typeClass}">
                    ${amountSign}${txn.amount.toFixed(2)} ብር
                </div>
            `;
            list.appendChild(li);
        });

        document.getElementById('total-cash').innerText = totalCash.toFixed(2) + ' ብር';
        document.getElementById('total-trans').innerText = totalTrans.toFixed(2) + ' ብር';
        document.getElementById('total-expense').innerText = totalExpense.toFixed(2) + ' ብር';
        document.getElementById('total-people').innerText = totalPeople + ' ሰው';

        const netBalance = (totalCash + totalTrans) - totalExpense;
        document.getElementById('net-balance').innerText = netBalance.toFixed(2) + ' ብር';
    }

    function escapeHtml(str) {
        const div = document.createElement('div');
        div.textContent = str;
        return div.innerHTML;
    }

    async function clearData() {
        if (confirm('እርግጠኛ ነህ ሁሉንም የተመዘገቡ መረጃዎች ማጥፋት ትፈልጋለህ?')) {
            transactions = [];
            await saveAndRender();
        }
    }
</script>

</body>
</html>
