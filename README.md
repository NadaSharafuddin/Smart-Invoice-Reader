# 🤖 Invoice Reader Robot – UiPath Automation

This UiPath robot is designed to intelligently read and extract key information from **PDF invoices that contain selectable text** 
(i.e., not scanned images or OCR-based). It can process a large number of invoices in one go, even if they come in **different layouts or formats**,
and automatically extracts essential data such as the **Invoice Number**, **Account Holder Name**, and **Invoice Amount**. All the extracted information is compiled into a single, 
well-organized Excel file saved in the **same folder** as the original invoices, making it easy to review and use the results.

## 📁 Folder Structure Example
Invoices/
├── invoice1.pdf
├── invoice2.pdf
└── Extracted_Invoice_Data.xlsx

## 🔧 Features

- ✅ Works with any PDF that contains readable (non-image) text
- ✅ Handles invoices with varying text layouts and formats
- ✅ Extracts Invoice Number, Account Holder Name, and Amount
- ✅ Outputs all extracted data into a single Excel file
- ✅ Ideal for batch processing of multiple PDF invoices

## 📦 Output Format

| File Name     | Invoice Number | Account Holder Name | Amount    |
|---------------|----------------|----------------------|-----------|
| invoice1.pdf  | INV-12345      | John Doe             | $1,200.00 |
| invoice2.pdf  | INV-67890      | Jane Smith           | $950.00   |

## 🚀 How to Use

1. Place all PDF invoices (with text) into a folder.
2. Open this project in UiPath Studio.
3. Run the robot.
4. The Excel file with the extracted data will be created in the same folder.

## 📌 Requirements

- UiPath Studio (latest version recommended)
- UiPath.PDF.Activities (for reading PDF text)
- One of the sequences in this InvoiceReader repository requires integration with UiPath Orchestrator in order to use the Generative AI Connector.

To run this part of the automation successfully, the user must:
- Have access to UiPath Orchestrator (Cloud or On-Premises)
- Create and configure a valid Orchestrator connection, this includes setting up Machine, Robot, and Environment properly.
- Enable the Generative AI Connector.. Available via UiPath Integration Service or Studio Web under the Connectors panel.
- If the Orchestrator connection is not established, this specific sequence may throw an error or fail to execute properly.

---

Developed with ❤️ using UiPath to automate invoice data extraction with speed and precision.

