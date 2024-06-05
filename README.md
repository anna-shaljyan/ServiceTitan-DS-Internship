# ServiceTitan-DS-Internship

### Task:
Write a DataExtractor class that has the functionality to load the dataset and transform the unstructured data into a flat data with the following columns:
- invoice_id: int
- created_on: datetime64[ns]
- invoiceitem_id: int
- invoiceitem_name: str
- type: str (use this conversion table: {0: 'Material', 1: 'Equipment', 2: 'Service', 3: 'Other'})
- unit_price: int
- total_price: int (unit_price*quantity)
- percentage_in_invoice: float (unit_price*quantity / invoice_total)
- is_expired: bool (whether invoice_id is contained expired_invoices.txt or not)

Make sure that the columns in the resulting dataframe are of the correct type, as described above. The final dataframe must be sorted by invoice_id and invoiceitem_id in the ascending order.

Once you complete the exercise - upload the following files to your Github repo:
- A jupyter notebook or an executable .py file, which contains the code
- The resulting dataframe in a .csv format, that exactly matches the above specification
