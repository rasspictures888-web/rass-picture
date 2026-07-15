<!DOCTYPE html>
<html lang="am">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RAS Pictures - Dashboard</title>
    <script src="https://accounts.google.com/gsi/client" async defer></script>
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
    </style>
</head>
<body>

<div class="container">
    <header>
        <h1>RAS PICTURES</h1>
        <p style="margin: 0; font-size: 12px; color: #aaa;">የዕለት የሂሳብ መቆጣጠሪያ</p>
    </header>

    <div class="auth-bar">
        <div id="signed-out-view">
            <p>ውሂብዎን በGoogle Drive ላይ ለማስቀመጥ እና በሁሉም መሳሪያዎችዎ ላይ ለማግኘት ይግቡ</p>
            <button class="btn-google" id="signin-btn">Google Sign-In</button>
        </div>
        <div id="signed-in-view" style="display:none;">
            <span class="signed-in-badge">✓ ተገናኝቷል: <span id="user-email"></span></span>
            <button class="btn-signout" id="signout-btn">ውጣ</button>
        </div>
    </div>

    <div id="app-content">
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
    const GOOGLE_CLIENT_ID = '123219683130-0tt5p7eku9uj8cggti7tm9ebe4276rip.apps.googleusercontent.com';
    const DRIVE_FILENAME = 'ras_pictures_transactions.json';
    const DRIVE_SCOPE = 'https://www.googleapis.com/auth/drive.file';

    let transactions = [];
    let accessToken = null;
    let driveFileId = null;
    let tokenClient = null;

    // ==== AUTH ====
    window.addEventListener('load', () => {
        tokenClient = google.accounts.oauth2.initTokenClient({
            client_id: GOOGLE_CLIENT_ID,
            scope: DRIVE_SCOPE,
            callback: async (response) => {
                if (response.error) {
                    console.error('Auth error:', response);
                    setSyncStatus('⚠ መግባት አልተቻለም');
                    return;
                }
                accessToken = response.access_token;
                await onSignedIn();
            }
        });

        document.getElementById('signin-btn').addEventListener('click', () => {
            tokenClient.requestAccessToken();
        });

        document.getElementById('signout-btn').addEventListener('click', signOut);
    });

    async function onSignedIn() {
        document.getElementById('signed-out-view').style.display = 'none';
        document.getElementById('signed-in-view').style.display = 'block';
        document.getElementById('app-content').style.display = 'block';

        try {
            const userInfoRes = await fetch('https://www.googleapis.com/oauth2/v2/userinfo', {
                headers: { Authorization: 'Bearer ' + accessToken }
            });
            const userInfo = await userInfoRes.json();
            document.getElementById('user-email').innerText = userInfo.email || '';
        } catch (e) {
            console.error('Could not fetch user info', e);
        }

        await loadData();
    }

    function signOut() {
        if (accessToken) {
            google.accounts.oauth2.revoke(accessToken, () => {});
        }
        accessToken = null;
        driveFileId = null;
        transactions = [];
        document.getElementById('signed-out-view').style.display = 'block';
        document.getElementById('signed-in-view').style.display = 'none';
        document.getElementById('app-content').style.display = 'none';
    }

    // ==== DRIVE FILE HELPERS ====
    async function findDriveFile() {
        const q = encodeURIComponent(`name='${DRIVE_FILENAME}' and trashed=false`);
        const res = await fetch(`https://www.googleapis.com/drive/v3/files?q=${q}&spaces=drive&fields=files(id,name,modifiedTime)`, {
            headers: { Authorization: 'Bearer ' + accessToken }
        });
        if (!res.ok) throw new Error('Drive search failed: ' + res.status);
        const data = await res.json();
        if (data.files && data.files.length > 0) {
            data.files.sort((a, b) => new Date(b.modifiedTime) - new Date(a.modifiedTime));
            return data.files[0].id;
        }
        return null;
    }

    async function createDriveFile(content) {
        const metadata = { name: DRIVE_FILENAME, mimeType: 'application/json' };
        const boundary = '-------314159265358979323846';
        const delimiter = "\r\n--" + boundary + "\r\n";
        const closeDelim = "\r\n--" + boundary + "--";

        const body =
            delimiter +
            'Content-Type: application/json\r\n\r\n' +
            JSON.stringify(metadata) +
            delimiter +
            'Content-Type: application/json\r\n\r\n' +
            content +
            closeDelim;

        const res = await fetch('https://www.googleapis.com/upload/drive/v3/files?uploadType=multipart&fields=id', {
            method: 'POST',
            headers: {
                Authorization: 'Bearer ' + accessToken,
                'Content-Type': 'multipart/related; boundary="' + boundary + '"'
            },
            body: body
        });
        if (!res.ok) throw new Error('Drive create failed: ' + res.status);
        const data = await res.json();
        return data.id;
    }

    async function updateDriveFile(fileId, content) {
        const res = await fetch(`https://www.googleapis.com/upload/drive/v3/files/${fileId}?uploadType=media`, {
            method: 'PATCH',
            headers: {
                Authorization: 'Bearer ' + accessToken,
                'Content-Type': 'application/json'
            },
            body: content
        });
        if (!res.ok) throw new Error('Drive update failed: ' + res.status);
    }

    async function downloadDriveFile(fileId) {
        const res = await fetch(`https://www.googleapis.com/drive/v3/files/${fileId}?alt=media`, {
            headers: { Authorization: 'Bearer ' + accessToken }
        });
        if (!res.ok) throw new Error('Drive download failed: ' + res.status);
        return await res.text();
    }

    // ==== DATA LOAD / SAVE ====
    async function loadData() {
        setSyncStatus('ከGoogle Drive በመጫን ላይ...');
        try {
            driveFileId = await findDriveFile();
            if (driveFileId) {
                const content = await downloadDriveFile(driveFileId);
                transactions = content ? JSON.parse(content) : [];
            } else {
                transactions = [];
                driveFileId = await createDriveFile('[]');
            }
            setSyncStatus('✓ ከGoogle Drive ጋር ተመሳስሏል');
        } catch (error) {
            console.error('Load error:', error);
            transactions = [];
            setSyncStatus('⚠ ከGoogle Drive መጫን አልተቻለም');
        }
        render();
    }

    async function saveAndRender() {
        submitBtn.disabled = true;
        submitBtn.innerText = 'ወደ Google Drive በመላክ ላይ...';
        setSyncStatus('በማስቀመጥ ላይ...');
        try {
            const content = JSON.stringify(transactions);
            if (!driveFileId) {
                driveFileId = await createDriveFile(content);
            } else {
                await updateDriveFile(driveFileId, content);
            }
            setSyncStatus('✓ ወደ Google Drive ተቀምጧል');
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
        if (!accessToken) return;

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
