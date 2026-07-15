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

        .btn-submit:hover {
            background: #333;
        }

        .btn-submit:disabled {
            opacity: 0.6;
            cursor: not-allowed;
        }

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

        .transaction-item:last-child {
            border-bottom: none;
        }

        .txn-details {
            display: flex;
            flex-direction: column;
        }

        .txn-date {
            font-size: 11px;
            color: #888;
        }

        .txn-people {
            font-size: 12px;
            color: #555;
            margin-top: 2px;
        }

        .txn-amount {
            font-weight: bold;
        }

        .income-cash { color: var(--success-color); }
        .income-trans { color: #0077b6; }
        .expense { color: var(--danger-color); }

        .empty-state {
            text-align: center;
            color: #999;
            padding: 20px;
            font-size: 14px;
        }

        .loading-state {
            text-align: center;
            color: #999;
            padding: 20px;
            font-size: 14px;
        }
    </style>
</head>
<body>

<div class="container">
    <header>
        <h1>RAS PICTURES</h1>
        <p style="margin: 0; font-size: 12px; color: #aaa;">የዕለት የሂሳብ መቆጣጠሪያ</p>
    </header>

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
            <li class="loading-state">ከGoogle Drive በመጫን ላይ...</li>
        </ul>
        <p id="sync-status" style="text-align:center; font-size:11px; color:#999; margin-top:10px;"></p>
    </div>
</div>

<script>
    const DRIVE_FILENAME = 'ras_pictures_transactions.json';
    const DRIVE_FILE_ID = '1u3kPojR35t_hlNNsjRTdgKs4K4fo0wYB';
    let transactions = [];

    async function callClaudeWithDrive(prompt) {
        const response = await fetch("https://api.anthropic.com/v1/messages", {
            method: "POST",
            headers: { "Content-Type": "application/json" },
            body: JSON.stringify({
                model: "claude-sonnet-4-6",
                max_tokens: 1000,
                messages: [{ role: "user", content: prompt }],
                mcp_servers: [
                    {
                        type: "url",
                        url: "https://drivemcp.googleapis.com/mcp/v1",
                        name: "google-drive"
                    }
                ]
            })
        });
        const data = await response.json();
        const textBlocks = (data.content || [])
            .filter(item => item.type === "text")
            .map(item => item.text);
        return textBlocks.join("\n").trim();
    }

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

    function setSyncStatus(msg) {
        const el = document.getElementById('sync-status');
        if (el) el.innerText = msg;
    }

    async function saveAndRender() {
        submitBtn.disabled = true;
        submitBtn.innerText = 'ወደ Google Drive በመላክ ላይ...';
        setSyncStatus('በማስቀመጥ ላይ...');
        try {
            const content = JSON.stringify(transactions);
            const prompt = `Use Google Drive tools to update the file with ID "${DRIVE_FILE_ID}" (named "${DRIVE_FILENAME}") so its content becomes exactly this JSON (there is no update tool, so create_file with the same title will be treated as the new version — just make sure only ONE current version has this new content):\n\n${content}\n\nAfter doing this, reply with only the word DONE.`;
            const result = await callClaudeWithDrive(prompt);
            if (result.includes('DONE')) {
                setSyncStatus('✓ ወደ Google Drive ተቀምጧል');
            } else {
                setSyncStatus('⚠ ማስቀመጥ ላይ ችግር ተፈጥሯል');
            }
        } catch (error) {
            console.error('Drive save error:', error);
            setSyncStatus('⚠ ከGoogle Drive ጋር መገናኘት አልተቻለም');
        }
        submitBtn.disabled = false;
        submitBtn.innerText = 'መዝግብ';
        render();
    }

    async function loadData() {
        setSyncStatus('ከGoogle Drive በመጫን ላይ...');
        try {
            const prompt = `Use Google Drive tools to download the content of the file with ID "${DRIVE_FILE_ID}". Reply with ONLY the raw JSON array it contains — no explanation, no markdown code fences, no extra text. If the file is empty or unreadable, reply with exactly: []`;
            const result = await callClaudeWithDrive(prompt);
            const cleaned = result.replace(/```json|```/g, '').trim();
            const parsed = JSON.parse(cleaned);
            transactions = Array.isArray(parsed) ? parsed : [];
            setSyncStatus('✓ ከGoogle Drive ጋር ተመሳስሏል');
        } catch (error) {
            console.error('Drive load error:', error);
            transactions = [];
            setSyncStatus('⚠ ከGoogle Drive መጫን አልተቻለም — ባዶ ዝርዝር ታይቷል');
        }
        render();
    }

    function render() {
        const list = document.getElementById('transaction-list');
        list.innerHTML = '';

        let totalCash = 0;
        let totalTrans = 0;
        let totalExpense = 0;
        let totalPeople = 0;

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

            let typeClass = '';
            let typeLabel = '';
            let amountSign = '+';

            if (txn.type === 'cash') {
                typeClass = 'income-cash';
                typeLabel = 'ካሽ';
            } else if (txn.type === 'transaction') {
                typeClass = 'income-trans';
                typeLabel = 'ትራንዛክሽን';
            } else {
                typeClass = 'expense';
                typeLabel = 'ወጪ';
                amountSign = '-';
            }

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
        if (confirm('እርግጠኛ ነህ ሁሉንም የተመዘገቡ መረጃዎች ማጥፋት ትፈልጋለህ? (አዲስ ባዶ ፋይል በGoogle Drive ላይ ይፈጠራል)')) {
            transactions = [];
            await saveAndRender();
        }
    }

    loadData();
</script>

</body>
</html>
