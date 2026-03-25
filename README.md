 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
index 96684cd46aa859c293625dc21a5730a70437c1cd..fa5f678f68c446b9e3989d1a151fce57cc2f1867 100644
--- a/README.md
+++ b/README.md
@@ -1 +1,24 @@
-# expenseApp
\ No newline at end of file
+# FlowLedger AI Expense App
+
+A lightweight, modern web app inspired by Numi for ultra-fast natural language financial tracking.
+
+## Features
+
+- Smart NLP-style parsing for expense, income, receivable, and payable entries.
+- Auto calculations (e.g. `five books each 130tk` -> `650tk`).
+- Debt/credit tracking with due-date extraction and reminders.
+- Editable ledger entries with settle/reopen actions.
+- Dashboard cards (income, expense, receivable, payable, net).
+- Spending analytics by category.
+- Search and filters for quick retrieval.
+- Local persistence with `localStorage`.
+
+## Run
+
+Because this is plain HTML/CSS/JS, you can run it with any static server:
+
+```bash
+python -m http.server 4173
+```
+
+Then open `http://localhost:4173`.
 
EOF
)
