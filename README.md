document.getElementById('total-trans').innerText = totalTrans.toFixed(2) + ' ብር';
        document.getElementById('total-expense').innerText = totalExpense.toFixed(2) + ' ብር';
        document.getElementById('total-people').innerText = totalPeople + ' ሰው';

        const netBalance = (totalCash + totalTrans) - totalExpense;
        document.getElementById('net-balance').innerText = netBalance.toFixed(2) + ' ብር';
    }

    // መረጃዎችን ሙሉ በሙሉ ለማጥፋት
    function clearData() {
        if (confirm('እርግጠኛ ነህ ሁሉንም የተመዘገቡ መረጃዎች ማጥፋት ትፈልጋለህ?')) {
            transactions = [];
            saveAndRender();
        }
    }

    // ገጹ ሲከፈት መረጃዎችን አውጥቶ እንዲያሳይ
    render();
</script>

</body>
</html>
