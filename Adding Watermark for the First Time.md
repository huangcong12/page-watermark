# Instructions
This document is the first demonstration of adding watermarks for the Shopify App [`LitaCat - Page Watermark`](https://apps.shopify.com/page-watermark).

| Description | Date |
| -- | -- |
| First Version | 2024-03-02|


-----------------------------------------------------------------

# Adding Watermark for the First Time
This is a simple tutorial to assist merchants in adding page watermarks to their store pages. The entire process takes about 5 minutes.

## Step 1: Embedding Theme Extension
Click on the menu and go to the Page Watermark List App page. A pop-up will appear, indicating that you need to open the plugin's theme extension. There are a total of 3 steps, and the last step is to click the "Save" button.
![image](https://github.com/huangcong12/page-watermark/assets/2867782/8d804f6b-4ca6-4498-b816-29239d4d56f5)


## Step 2
Return to the list page and click on "Generate a Watermark" in the upper right corner.
![image](https://github.com/huangcong12/page-watermark/assets/2867782/cc48b6ed-5708-4045-942e-173e38186fce)



## Step 3: Editing Watermark Information
After entering the "Generate a Watermark" page, you may need to pay attention to 4 areas:
- Title: The title helps merchants remember the purpose of this watermark. The title is unique within the same store. If it's the first time adding, you can use the default value.
- Sort: The sequence number of the rule. The higher the number, the higher it is displayed. When a page matches multiple watermark records, the one with the highest sequence number is used. To avoid confusion, Sort is also designed to be unique within the same store. If it's the first time adding, you can use the default value.
- Effective URLs: URLs where the watermark will be applied. Simply copy and paste the URL directly from the browser. For example, if the address of a product in my store is: `https://quickstart-7bdd85a9.myshopify.com/products/the-collection-snowboard-liquid`, then I directly paste this address into the Effective URLs column. If you want all product pages to display the watermark, change it to `https://quickstart-7bdd85a9.myshopify.com/products/*` for full matching. If you want all pages to display the watermark, simply enter `*` to match all pages.
- Text Content: The content of the watermark. For example, I have added "Promotional product" and then found the font size too small, so I changed the "Size" from 10 to 20.
![image](https://github.com/huangcong12/page-watermark/assets/2867782/2ddd33e3-4966-484b-8e95-121bc53db084)

Then click the "Save" button at the bottom of the browser. If there are no prompts, it means the save was successful. Finally, refresh `https://quickstart-7bdd85a9.myshopify.com/products/the-collection-snowboard-liquid` to see the watermark appear on the page.
![image](https://github.com/huangcong12/page-watermark/assets/2867782/77fe928c-58d0-4d05-abff-6d5b3c8d50da)



---------------------------------------
Next steps:
- For managing watermarked images, please refer to [Managing Watermarked Images](https://github.com/huangcong12/page-watermark/blob/main/Managing%20Watermark%20Images.md).
- For more parameter configurations, please refer to the document [Analysis of Watermark Configuration Parameters](https://github.com/huangcong12/page-watermark/blob/main/Analysis%20of%20Watermark%20Configuration%20Parameters.md).
