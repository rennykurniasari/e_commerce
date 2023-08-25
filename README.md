# Final Project FGA DTS 2023 - BDP SAMRAT B - Kelompok 1

## Anggota Kelompok:
1. Adittya Kamal Mahardin
2. Renny Kurniasari
3. Theresia Rosaria
4. Tegar Kamarulzaman
5. Semmy Vigmendelson K

## Case Objective
1. How much sales for each category ?
2. How much the average order value for each year ?
3. Which category & product makes the most profit ?
4. Which product had worst growth in books category for each year ?
5. Who are the best customers?
6. Who has the potential to become valuable customers?

## Dependencies
*   `pip install pandas`
*   `pip install numpy`
*   `pip install matplolib`
*   `pip install seaborn`
*   `pip install plotly`
*   `pip install hvplot`
*   `pip install panel`
*   `pip install holoviews`

---


## Data Dictionary

Source: https://www.kaggle.com/datasets/rennykurniasari/e-commerce-dataset

> **Order Detail**

|variable                       |class     |description |
|:------------------------------|:---------|:-----------|
id 			|object| angka unik dari order / id_order
customer_id 		|object|angka unik dari pelanggan
order_date 		|object| tanggal saat dilakukan transaksi
sku_id 			|object| angka unik dari produk (sku adalah stock keeping unit)
price			|int64| harga yang tertera pada tagging harga
qty_ordered 		|int64| jumlah barang yang dibeli oleh pelanggan
before_discount	|float64| nilai harga total dari produk (price * qty_ordered)
discount_amount	|float64| nilai diskon product total
after_discount		|float64| nilai harga total produk ketika sudah dikurangi dengan diskon
is_gross 		|int64| menunjukkan pelanggan belum membayar pesanan
is_valid		|int64| menunjukkan pelanggan sudah melakukan pembayaran
is_net			|int64| menunjukkan transaksi sudah selesai
payment_id 		|int64| angka unik dari metode pembayaran

> **SKU Detail**

|variable                       |class     |description |
|:------------------------------|:---------|:-----------|
id |object| angka unik dari produk (dapat digunakan untuk key saat join)
sku_name 		|object| nama dari produk
base_price		|float64| harga barang yang tertera pada tagging harga / price
cogs 			|int64| cost of goods sold / total biaya untuk menjual 1 produk
category		|object| kategori produk

> **Customer Detail**

|variable                       |class     |description |
|:------------------------------|:---------|:-----------|
id 			|object| angka unik dari pelanggan
registered_date	|object| tanggal pelanggan mulai mendaftarkan diri sebagai anggota

> **Payment Detail**

|variable                       |class     |description |
|:------------------------------|:---------|:-----------|
id			|int64| angka unik dari metode pembayaran
payment_method	|object| metode pembayaran yang digunakan
