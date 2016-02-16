===============
Accounting Odoo
===============

Halaman ini berisi rangkuman mengenai bagaimana Odoo mengatur Akun dan transaksi.

Double-entry bookkeeping
========================

Odoo secara otomatis akan membuat journal untuk setiap transaksi keuangan, seperti
penerbitan invoice (AR), penerimaan billing (AP), perpindahan barang, pembayaran dll.

Odoo menggunakan aturan sistem double-entry bookkeeping yang artinya semua journal entries
akan secara otomatis dibuat balance (jumlah Debit = jumlah Credit).

.. seealso::

	`Understand Odoo's accounting transactions per document <https://odoo.com/documentation/functional/accounting.html>`__

Accrual and Cash Basis Methods
==============================

Odoo mensupport baik accrual basis maupun cash basis. Hal ini memungkinkan pengguna
untuk melaporkan Expense / Income pada saat transaksi (accrual basis) atau pada saat pembayaran diterima (cash basis)

Multi-companies
===============

Odoo memungkinkan untuk mengatur beberapa perusahaan dalam satu database.
Setiap perusahaan akan mempunyai chart of account sendiri dan aturan sendiri.
Anda akan mendapatkan laporan konsolidasi sesuai dengan aturan yang ditetapkan.

Pengguna yang diberikan akses dapat mengatur beberapa perusahaan, tetapi hanya bisa bekerja
pada 1 perusahaan pada saat yang bersamaan.

Multi-currencies
================

Setiap transaksi akan dicatat dalam Mata Uang basis (Functional Currency). Setiap 
transaksi yang menggunakan mata uang lain, Odoo akan menyimpannya dalam 2 nilai
yaitu dalam functional currency dan original currency. Odoo dapat menghasilkan 
laba/rugi kurs setelah ada rekonsiliasi pada journal item.

Nilai kurs dapat diperbaharui setiap hari menggunakan web-service dari yahoo.com

International Standards
=======================

Accounting Odoo mensupport lebih dari 50 negara. Dasar Accounting Odoo mengadopsi 
standar akutansi yang berlaku umum dan tersedia modul spesifik per negara seperti COA, Pajak dan atau Bank interface.
Databit sebagai Official Odoo Partner, telah membuat modul2 spesifik yang sesuai dengan
peraturan akutansi di Indonesia.

Modul-modul spesifi lain :

* Anglo-Saxon Accounting (U.S., U.K.,, and other English-speaking
  countries including Ireland, Canada, Australia, dan New Zealand)
  dimana HPP dilaporkan ketika produk dijual atau di kirim.
* European accounting dimana Expenses diposting ketika loading AP.
* Storno accounting (Italy) dimana retur mempunyai nilai negatif pada Debit/Credit 
  dibandingkan dengan membuat journal balik.

Odoo juga mempunyai modul yang sesuai dengan IFRS.

Accounts Receivable & Payable
=============================

Secara default, Odoo menggunakan 1 account untuk semua AR dan AP. Pengguna dapat membuat 
akun AR per masing Customer, atau akun AP per masing2 Supplier, tapi hal ini tidak dibutuhkan, karena 
Odoo menyediakan laporan AR ato AP per masing2 Customer/Supplier.

Setiap transaksi yang berkaitan dengan Customer atau Supplier, dapat ditampilkan dalam laporan 
per masing-masing customer/supplier tersebut.

Baru sampai sini
================

Wide range of financial reports
===============================

In Odoo, you can generate financial reports in real time. Odoo's
reports range from basic accounting reports to advanced management
reports. Odoo's reports include:

* Performance reports (such as Profit and Loss, Budget Variance)
* Position reports (such as Balance Sheet, Aged Payables, Aged
  Receivables)
* Cash reports (such as Bank Summary)
* Detail reports (such as Trial Balance and General Ledger)
* Management reports (such as Budgets, Executive Summary)

Odoo's report engine allows you to customize your own report based on
your own formulae.

Import bank feeds automatically
===============================

Bank reconciliation is a process that matches your bank statement
lines, as supplied by the bank, to your accounting transactions in the
general ledger. Odoo makes bank reconciliation easy by frequently
importing bank statement lines from your bank directly into your Odoo
account. This means you can have a daily view of your cashflow without
having to log into your online banking or wait for your paper bank
statements.

Odoo speeds up bank reconciliation by matching most of your imported
bank statement lines to your accounting transactions. Odoo also
remembers how you've treated other bank statement lines and provides
suggested general ledger transactions.

Calculates the tax you owe your tax authority
=============================================

Odoo totals all your accounting transactions for your tax period and
uses these totals to calculate your tax obligation. You can then check
your sales tax by running Odoo's Tax Report.

Inventory Valuation
===================

Odoo support both periodic (manual) and perpetual (automated)
inventory valuations. The available methods are standard price,
average price, LIFO (for countries allowing it) and FIFO.

.. seealso::

	`View impact of the valuation method on your transactions <https://odoo.com/documentation/functional/valuation.html>`__

Easy retained earnings
======================

Retained earnings is the portion of income retained by your
business. Odoo automatically calculates your current year earnings in
real time so no year-end journal or rollover is required.  This is
calculated by reporting the profit and loss balance to your balance
sheet report automatically.
