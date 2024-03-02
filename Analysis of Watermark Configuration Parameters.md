# Description
This document is an analysis of all parameters on the editing page of the Shopify App [`LitaCat - Page Watermark`](https://apps.shopify.com/page-watermark).

| Description | Date |
| -- | -- |
| First Version | 2024-03-02 |

----------------------------------------------------------------------
# Title
The title serves to help merchants remember the purpose of this watermark. Within the same store, the title is unique. If it's the first time adding, you can use the default value.

# Status
The status has two options: Enable and Disable. Only watermarks with "Enabled" status will take effect. If you wish to hide a watermark, change it to "Disabled".
![image](https://github.com/huangcong12/page-watermark/assets/2867782/7e10fe04-cd29-48eb-b812-1b9cf896d11d)

# Sort
The sequence number of the rule, supports 1 to 99999. The higher the number, the higher it's displayed. For example, 99999 is the highest, and 1 is the lowest. When a page matches multiple watermark records, the one with the highest sequence number is applied. To avoid confusion, Sort is also unique within the same store. If it's the first time adding, you can use the default value.

# Vertical Spacing
The vertical spacing between watermarks, default is 50.
| Parameter Value | Effect |
| -- | -- |
| 50 | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/0ed92351-04d6-4e09-9ce0-1a196d49657e) |
| 150 | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/ec5e6ebe-4e37-4a02-b14c-f5044d031024) |

# Horizontal Spacing
The horizontal spacing between watermarks, default is 50.
| Parameter Value | Effect |
| -- | -- |
| 50 | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/b6e82832-7da2-4e2b-932d-94c34ceda0d6) |
| 150 | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/029a2e6d-288b-403a-afad-06ad569758b3) |

# Watermark Generation Type
The display method of watermarks, supporting two types.
![image](https://github.com/huangcong12/page-watermark/assets/2867782/1c41e4a3-49fe-42ea-a57f-fea86d3282a9)

| Parameter Value | Demo |
| -- | -- |
| TileAcrossPage: Tiles across the entire page, somewhat similar to the desktop setting of Windows 98. | Default. |
| SingleCentered: Only one watermark is centered. If you choose this option, you may need to adjust the font size and opacity to attract user attention. | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/93014ff0-c755-4121-af0d-d6c1b4ca42d5) |

# Rotate Angle
The rotation angle of the watermark, supports 0~360, default is 45.
| Parameter Value | Effect |
| -- | -- | 
| 0: No tilt angle. | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/2d7dcd36-6189-48b4-a993-f03bdf575147) |
| 45: Tilted 45°. | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/71d1e261-7c1d-440e-8482-e9306886f8a6) |
| 90: Tilted 90°. | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/2f56609b-dfb5-410b-9b81-10544adf4be4) |
| 180: Tilted 180°. | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/d979172e-1d81-45cc-91e3-e32bc518a447) |

# Effective URLs
The collection of URLs where the rule takes effect.
#### Exact Match
Paste the complete URL here to apply the watermark to the product page. For example: `https://quickstart-7bdd85a9.myshopify.com/products/the-3p-fulfilled-snowboard`![image](https://github.com/huangcong12/page-watermark/assets/2867782/21275811-545f-4562-b166-9eae0f0cd55d)

#### `*` Wildcard
| Parameter Value | Demo |
| -- | -- |
| If you want all pages to display the watermark, just enter `*`. | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/1e1d6660-32b7-4f99-b128-92569dab3325) |
| If you want all product pages to display the watermark, enter `https://{Your Shop Domain}/products/*`, for example, mine is `https://quickstart-7bdd85a9.myshopify.com/products/*`. | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/ea6522b5-0ae2-4785-af22-790100b06d7a) |

#### Multiple Match
Simply paste multiple URLs, one per line. For example, if you want two product detail pages to display the watermark, just copy and paste the addresses of those two products.
![image](https://github.com/huangcong12/page-watermark/assets/2867782/6bcfb93d-ee41-40f5-8cae-8d64b940f168)

# Exclude URLs
The collection of URLs where the watermark should not be displayed. For example, if you used the wildcard `*` in the "Effective URLs" to display the watermark on all pages, but you want `https://quickstart-7bdd85a9.myshopify.com/pages/contact` to not display the watermark, then enter `https://quickstart-7bdd85a9.myshopify.com/pages/contact` in Exclude URLs. It will skip the current rule and continue to match subsequent rules. Like Effective URLs, it supports exact match, `*` wildcard, and multiple lines.
![image](https://github.com/huangcong12/page-watermark/assets/2867782/f8e03e38-1be4-4286-bcc3-a9e85c1c8e90)

# Effective Start Time (Optional)
The start time for the rule to take effect. Time is based on the user's browser time. Due to

 different time zones around the world, the displayed time varies. For example: Set to start at AM 8:00, then it will first appear to users in Japan at AM 8:00, but users in Europe and the US will not see it at that time. Therefore, you cannot use it for flash sale type activities. Leave it blank for no time restriction, it will always be effective.

# Effective End Time (Optional)
The end time for the rule. Time is based on the user's browser time.

The time display format is different between Chrome and Firefox. In Chrome, you can select the specific time with the mouse.
| Parameter Value | Demo |
| -- | -- |
| Chrome: Simply select with the mouse. | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/3379e357-aa59-49a9-a64d-6dbd75c30730) |
| Firefox: The mouse intelligently selects the date, and you need to manually enter the H:i part. | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/15fe552c-798e-4e2c-9181-e3406140fffe) |

--------------------------------------------------------------------
# Text Content
The textual information of the watermark, supports line breaks. Supports emoji text expressions.
![image](https://github.com/huangcong12/page-watermark/assets/2867782/ef4b58a2-47a8-49b8-a0da-c3e2da440b6e)
![image](https://github.com/huangcong12/page-watermark/assets/2867782/8455096d-0beb-4b1f-8e2c-ccfa401676b6)

# Text Align
You can ignore this property for now.

# Size
The size of the font. If you find the font too small, adjust this.

# Line Spacing
Line height, default is 1.2.
| Parameter Value | Effect |
| -- | -- |
| 1.2 | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/9d56a1e0-2f15-48bd-a646-4ba9bcc88cc3) |
| 12 | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/952399a9-154b-4b96-a06b-bded0f110342) |

# Alpha
Opacity: 0.1~1. 1 is opaque.
| Parameter Value | Effect |
| -- | -- |
| 0.1 | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/44d76021-5184-4d56-b7d3-b9d86677c167) |
| 0.5 | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/1329a31b-f198-41a7-8ceb-d0ac8acb35d1) |
| 1 | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/aab8ad19-100e-4a2c-b031-0dcf3649282d) |

# Text Color
The color of the text.

--------------------------------------------------------------------

# Image URL
The URL of the image. Sometimes images may not be displayed immediately, save and refresh the page to check.

# Monochrome Display with Text Color
Whether to change the color of the image to match the text color. Suitable for SVG format images like logos, complex image effects may not look good, you can try it out.

# Height
The height of the image.

# Width
The width of the image.

# Image Position Relative to Text
The position of the image relative to the text, there are a total of 5 options:
![image](https://github.com/huangcong12/page-watermark/assets/2867782/10b1fc07-1057-4603-b74d-ac8bb2d5310c)

| Value | Description | Example |
| -- | -- | -- |
| Top | Image at the top of the text | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/f213d00b-e7e8-4f49-9a24-4e98cf978da8) |
| Right | Image to the right of the text | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/8a0bfcfa-ac50-4f47-88ae-6d56db144491) |
| Bottom | Image below the text | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/09b3e7a8-2ce3-4ce0-82c7-f4d2017eb912) |
| Left | Image to the left of the text | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/962efdac-521d-41c8-afda-179d0e4eeac8) |
| Center | Image in the center of the text | ![image](https://github.com/huangcong12/page-watermark/assets/2867782/531fbce3-5616-4f24-859f-6122672aa1a0) |
