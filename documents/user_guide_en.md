
# 2.0 plugin user guide

<div class="container-toc"></div>


## 1 About idealo

idealo started business in 2000 with the vision of helping users to make the right choices when buying products online and, now counting 50,000 sellers and 18 million users per month, has become one of Germany's most important e-commerce websites.<br/>

With idealo Checkout, idealo offers a strong sales channel. The "Zum Kauf" (Buy now) button allows users to order a product directly from idealo, using a fully integrated checkout function. The sellers remain the contractual partners and take care of fulfilment as usual.<br/>

#### idealo price comparison and idealo Checkout

With plentymarkets, you can both use the idealo price comparison and idealo Checkout (idealo's checkout function). If you set up idealo Checkout, you enable your customers to buy your products directly at idealo without having to enter your online store.


## 2 Registering with idealo

You have to register as a seller with idealo to set up the market in plentymarkets.

<div class="alert alert-warning" role="alert">
<b>Note: Item data export</b><br/> Inform idealo about how item data should be transferred before setting up idealo in plentymarkets (creating, updating, and deleting items on idealo). Item data can either be exported with a CSV file or via API (PWS 2.0 interface).<br/>
If you export your items with PWS 2.0, items will be created and deleted on idealo once a day. Prices and stock are updated every 15 minutes.<br/>
If you export your items with a CSV file using the elastic export, your items can be retrieved by idealo via URL.
 </ul>
</div>


#### 2.1 Installing the Elastic Export plugin

In order to use the idealo plugin, you have to install the [Elastic Export](https://marketplace.plentymarkets.com/en/plugins/sales/marktplaetze/elasticexport_4763) plugin first. You can download the plugin in the [plentyMarketplace](https://marketplace.plentymarkets.com/en).


## 3 Going through the idealo assistant

Go through the **idealo Basic settings** assistant in the **Setup » Assistants » Omni-Channel** menu to carry out the basic settings for idealo in plentymarkets. With this assistant, you set up your idealo account in plentymarkets and carry out settings for the item data export to idealo and order import from idealo Checkout.<br/>

<div class="alert alert-warning" role="alert">
<b>Note: Item data export via API</b><br/>It is mandatory to go through the <b>idealo Basic settings</b> assistant if you export your items to idealo with PWS 2.0. The automatic item export can only be set up in this assistant.
 </ul>
</div>


#### idealo price comparison and idealo Checkout

Depending on whether you only want to use the idealo price comparison or whether you want to enable your customers to buy items directly at idealo without having to enter your online store, different settings must be carried out. The overview below lists the settings required for idealo Checkout.

→ **Settings for idealo Checkout:**
- **Basic settings:** Go through the **idealo Basic settings** assistant in the **Setup » Assistants » Omni-Channel** menu.
- **Item export:** Set up the [automatic item export](#Item export via API) or the [item export via CSV file](#Item export with elastic export), je nachdem, depending on how you want to export your items to idealo.
- **Order referrer:** In addition to the order referrer **idealo**, also activate the [order referrer](#Activating the order referrer) **idealo Checkout** in the **Setup » Orders » Order referrer** menu.
- **Item availability:** In addition to the option **idealo**, also activate the [availability](#Setting the item availability) **idealo Checkout** in the **Item » Edit item » Open item » Tab: Variation ID » Tab: Availability** menu in the **Markets** section.
- **Sales price:** Set up a [sales price](#Defining a sales price).
- **SKU:** Add [SKUs](#Defining SKU manually) if needed.
- **Payment method:** Activate the [payment method](#Activating the payment method idealo Direktkauf) **idealo Direktkauf**.
- **Merkmale:** Create [characteristics](#Creating characteristics) for idealo Checkout. With characteristics, you can transfer item properties, shipping methods and charges to idealo Checkout.
- **Event procedures:** Set up [event procedures](#Setting up event procedures) to automatically inform idealo Checkout about changes in the order status.


## 4 Activating the order referrer
<a name="Activating the order referrer"></a>

In order to link items, characteristics etc. with the idealo price comparison portal, you have to activate the idealo order referrer in the **Setup » Orders » Order referrer** menu.

#### Activating the order referrer for the idealo price comparison:

1. Go to **Setup » Orders » Order referrer**.
2. Place a check mark next to **idealo**.
3. **Save** the settings.

If you would like to use idealo Checkout, then also activate the order referrer **idealo Checkout**.


## 5 Setting the item availability
<a name="Setting the item availability"></a>

Items have to be available for idealo. This is done in the **Availability** tab of an item within the **Item » Edit item » Open item » Tab: Variation ID** menu. Activate the item availability for idealo as described below.

#### Setting the item availability for the idealo price comparison:

1. Go to **Item » Edit item » Open item » Tab: Variation ID » Tab: Settings**.
2. Activate the main variation in the **Availability** section.
3. Click on the **Availability** tab.
4. Click in the selection field in the **Markets** section.<br/>
→ A list with all available markets is displayed.
5. Activate the option **idealo**.
6. Activate the option **Web API**.
7. Click on **Add**.<br/>
→ The market is added.
8. **Save** the settings.

The availability for variations can be edited in the **Item » Edit item » Open item » Tab: Variations » Open variation » Tab: Variation ID » Tab: Availability** menu.

If you want to use idealo Checkout, then also activate the order referrer **idealo Checkout** in the Markets section. If you activate the order referrer **idealo Checkout**, then the column **checkout_approved** is set to **true** in the CSV file that is generated in the elastic export.


## 6 Defining a sales price
<a name="Defining a sales price"></a>

Proceed as described below to define a sales price for the order referrer idealo. This price is displayed on idealo. It is valid for the idealo price comparison and idealo Checkout.

#### Defining a sales price for idealo:

1. Go to **Setup » Item » Sales prices » Open sales price » Tab: Settings**.<br/>
→ If you have not yet created a sales price, click on **New** to create a sales price.
2. Place a check mark next to the referrer **idealo**.
3. **Save** the settings.

<div class="alert alert-warning" role="alert">
<b>Note: Minimum price</b><br/>If you want to use a minimum price for idealo, then you have to define at least two sales prices for idealo: a minimum price and a standard sales price. The minimum price must have the price type <b>Special offer</b> and must be activated to the referrer <b>idealo Direktkauf</b>.<br/>
Which price should be transferred to idealo as minimum price is defined with the setting <b>Which price would you like to transfer to idealo as minimum price?</b> in the <b>Item data</b> step of the idealo assistant.
 </ul>
</div>


## 7 Defining SKU manually
<a name="Defining SKU manually"></a>

Add SKUs manually for specific referrers in the **Item » Edit item » Open item » Tab: Variation ID » Tab: Availability** menu if needed.

#### Adding SKU:

1. Go to **Item » Edit item » Open item » Tab: Variation ID » Tab: Settings**.
2. Click on the **Availability** tab.
3. Click on **Add** in the **SKU** section.<br/>
→ The **New SKU** window is displayed.
4. Select the referrer **idealo**.
5. Enter the SKU
6. Click on **Add**.<br/>
→ The SKU is saved and displayed.

If you want to use idealo Checkout, also add SKUs with the referrer **idealo Direktkauf**.


## 8 Setting up the item export

Items can be transferred to idealo with the automatic item export via API (PWS 2.0 interface) or via a CSV file with the elastic export. Depending on how you want to transfer your items to idealo, different settings are required.<br/>

→ **Note:** Inform idealo about how item data should be transferred before the setup in plentymarkets.

Information about the different types of data transfer is available in the following table:

|**Item export via API**        |**Item export via elastic export** |
|:---                           |:--- |
|Item data export via interface |Item data export via CSV file |
|Daily item updates             |Retrieval of item data via URL that is saved at idealo |
|Price updates every 15 minutes |Time interval for retrieval of item data is defined by idealo |
|Stock updates every 15 minutes | |


### 8.1 Item export via API (PWS 2.0 interface)
<a name="Item export via API"></a>

If you want to transfer your items to idealo via API, gp through the **idealo Basic settings** assistant in the **Setup » Assistants » Omni-Channel** menu and activate the automatic item data export. Apart from the assistant, no further settings are required to set up the automatic item export in plentymarkets.<br/>

If you transfer your items via API, items will be created and deleted at idealo once per day. Prices and stock will be updated every 15 minutes.


### 8.2 Item export with elastic export
<a name="Item export with elastic export"></a>

If you export items via the elastic export, you have to carry out a few settings in the **Data » Elastic export** menu to set up the export format. In order to use the elastic export, the [Elastic Export](https://marketplace.plentymarkets.com/en/plugins/sales/marktplaetze/elasticexport_4763) plugin must be installed in your plentymarkets system. First create the data format IdealoDE and afterwards transfer the URL to idealo so that idealo will be able to retrieve your item data.<br/>

How to set up the elastic export to export your items to idealo is described in the following chapters [Setting up the data format IdealoDE plugin in plentymarkets](#Setting up the data format IdealoDE plugin in plentymarkets) and [Available columns for the export file](#Available columns for the export file).


### 8.2.1 Setting up the data format IdealoDE plugin in plentymarkets
<a name="Setting up the data format IdealoDE plugin in plentymarkets"></a>

<div class="alert alert-warning" role="alert">
<b>Note: Settings only for elastic export</b><br/>The settings described in this chapter only need to be carried out if you transfer your items to idealo with the elastic export.
 </ul>
</div>

<div class="alert alert-warning" role="alert">
<b>Note: Check idealo product CSV</b><br/>Not all of the columns of idealo's product CSV are available in plentymarkets at present. Check whether you need columns which are not yet available in plentymarkets prior to setting up idealo in plentymarkets. In this case, an integration of idealo is currently not possible.<br/> An overview of the columns which are available in plentymarkets can be found in the <b>Available columns for the export file]</b> chapter.
 </ul>
</div>

Set up the export format **IdealoDE** so that your items can be exported to idealo with the elastic export. For further information about the elastic export, refer to the [Elastic Export](https://knowledge.plentymarkets.com/en/data/exporting-data/elastic-export) page of the plentymarkets manual.

#### Creating a new export format:

1. Go to **Data » Elastic export**.
2. Click on **New export**.
3. Carry out the settings as desired. Pay attention to the explanations given in table 1.
4. **Save** the settings.<br/>
→ The export format is given an ID and it appears in the overview within the **Exports** tab.

The following table lists details for settings, format settings and recommended item filters for the format **IdealoDE plugin**.

| **Setting**                                           | **Explanation** |
| :---                                                  | :--- |
| **Settings**                                          | |
| **Name**                                              | Enter a name. The export format will be listed under this name in the overview within the **Exports** tab. |
| **Type**                                              | Select the type **Item** from the drop-down list. |
| **Format**                                            | Select **IdealoDE-Plugin**. |
| **Limit**                                             | Enter a number. If you want to transfer more than 9,999 data records to the price search engine, then the output file will not be generated again for another 24 hours. This is to save resources. If more than 9,999 data records are necessary, the setting **Generate cache file** has to be active. |
| **Generate cache file**                               | Place a check mark if you want to transfer more than 9,999 data records to the price search engine. The output file will not be generated again for another 24 hours. We recommend not to activate this setting for more than 20 export formats. This is to save resources. |
| **Provisioning**                                      | Select **URL**. |
| **File name**                                         | The file name must have the ending **.csv** or **.txt** for idealo.de to be able to import the file successfully. |
| **Token, URL**                                        | If you have selected the option **URL** under **Provisioning**, then click on **Generate token**. The token will be entered automatically. When the token is generated under **Token**, the URL is entered automatically. |
| **Item filters**                                      | |
| **Add item filters**                                  | Select an item filter from the drop-down list and click on **Add**. There are no filters set in default. It is possible to add multiple item filters from the drop-down list one after the other.<br/> **Variations** = Select **Transfer all** or **Only transfer main variations**.<br/> **Markets** = Select **idealo**.<br/> The availability for all markets selected here has to be saved for the item. Otherwise, the export will not take place.<br/> **Currency** = Select a currency.<br/> **Category** = Activate to transfer the item with its category link. Only items belonging to this category will be exported.<br/> **Image** = Activate to transfer the item with its image. Only items with images will be transferred.<br/> **Client** = Select client.<br/> **Stock** = Select which stocks you want to export.<br/> **Flag 1 - 2** = Select the flag.<br/> **Manufacturer** = Select one, several or **ALL** manufacturers.<br/> **Active** = Only active variations will be exported. |
| **Format settings**                                   | |
| **Product URL**                                       | Choose wich URL should be transferred to the price comparison portal, the item’s URL or the variation’s URL. Variation SKUs can only be transferred in combination with the Ceres store. |
| **Client**                                            | Select a client. This setting is used for the URL structure. |
| **URL parameter**                                     | Enter a suffix for the product URL if this is required for the export. If you have activated the transfer option for the product URL further up, then this character string will be added to the product URL. |
| **Order referrer**                                    | Choose the order referrer **idealo**. The selected referrer is added to the product URL so that sales can be analysed later. |
| **Marketplace account**                               | Select the marketplace account from the drop-down list. |
| **Language**                                          | Select the language from the drop-down list. |
| **Item name**                                         | Select **Name 1**, **Name 2** or **Name 3**. These names are saved in the **Texts** tab of the item. Enter a number into the **Maximum number of characters (def. Text)** field if desired. This specifies how many characters should be exported for the item name. |
| **Preview text**                                      | Select the text that you want to transfer as preview text.<br/> Enter a number into the **Maximum number of characters (def. text)** field if desired. This will specify how many characters should be exported for the item name.<br/> Activate the option **Remove HTML tags** if you want HTML tags to be removed during the export.<br/> If you only want to allow specific HTML tags to be exported, then enter these tags into the field **Permitted HTML tags, separated by comma (def. Text)**. Use commas to separate multiple tags. |
| **Description**                                       | Select the text that you want to transfer as description.<br/> Enter a number into the **Maximum number of characters (def. text)** field if desired. This specifies how many characters should be exported for the description.<br/> Activate the option **Remove HTML tags** if you want HTML tags to be removed during the export. If you only want to allow specific HTML tags to be exported, then enter these tags into the field **Permitted HTML tags, separated by comma (def. Text)**. Use commas to separate multiple tags. |
| **Target country**                                    | Select the target country from the drop-down list. |
| **Barcode**                                           | Select the ASIN, ISBN or an EAN from the drop-down list. The barcode has to be linked to the order referrer selected above. If the barcode is not linked to the order referrer it will not be exported. |
| **Image**                                             | Select **Position 0** or **First image** to export this image.<br/> **Position 0** = An image with position 0 will be transferred.<br/> **First image** = The first image will be transferred. |
| **Image position of the energy efficiency label**     | Enter the position. Every image that should be transferred as an energy efficiency label must have this position. |
| **Stockbuffer**                                       | The stock buffer for variations with the limitation to the net stock. |
| **Stock for variations without stock limitation**     | The stock for variations without stock limitation. |
| **Stock for variations with no stock administration** | The stock for variations without stock administration. |
| **Live currency conversion**                          | Activate this option to convert the price into the currency of the selected country of delivery. The price has to be released for the corresponding currency. |
| **Retail price**                                      | Select gross price or net price from the drop-down list. |
| **Offer price**                                       | This option does not affect this format. |
| **RRP**                                               | Activate to transfer the RRP. |
| **Shipping costs**                                    | The chosen payment method does not affect this format. All payment methods of the selected configuration will be exported.<br/> If no configuration has been selected, all configurations and payment methods will be exported.<br/> If **Transfer flat rate shipping charge** has been selected, only prepayment will be exported as the payment method. |
| **VAT note**                                          | This option does not affect this format. |
| **Item availability**                                 | Activate the **overwrite** option and enter item availabilities into the fields **1** to **10**. The fields represent the IDs of the availabilities. This will overwrite the item availabilities that are saved in the menu **System » Item » Availability**. |

_Tab. 1: Settings for the export format IdealoDE_

### 8.2.2 Available columns for the export file
<a name="Available columns for the export file"></a>

| **Column description**  | **Explanation** |
| :---                    | :--- |
| **article_id**          | **Required**<br/> The **SKU** of the item. For all items which are configured for **idealo Checkout** a SKU will be generated for **idealo Checkout**. |
| **deeplink**            | **Required**<br/> The **URL** of the item depending on the selected **Client** in the format settings. |
| **name**                | **Required**<br/> According to the format setting **Item name**.|
| **short_description**   | According to the format setting **Preview text**. |
| **description**         | **Limitation**: max. 1000 characters<br/> According to the format setting **Description**. |
| **article_no**          | The **Variation number** within **Item » Edit item » Open item » Open variation » Settings » Basic settings**. |
| **producer**            | The **Name of the manufacturer** of the item. The **external name** within **Setup » Item » Manufacturer** will be preferred, if existing. |
| **model**               | The **Model** within **Items » Edit items » Open item » Open variation » Settings » Basic settings**. |
| **availability**        | **Required**<br/> The **Name of the item availability** within **Setup » Item » Item availability** or the translation according to the format setting **Overwrite item availability**. |
| **ean**                 | According to the format setting **Barcode**. |
| **isbn**                | According to the format setting **Barcode**. |
| **fedas**               | The **Amazon product type** within **Items » Edit item » Open item » Multi-Channel » Amazon**. |
| **warranty**            | Currently not configured. |
| **price**               | **Required**<br/> The **retail price** of the variation. |
| **price_old**           | The **retail price** of type **RRP** of the variation, if activated in the format settings. |
| **weight**              | The **gross weight** in gram within **Items » Edit item » Open item » Open variation » Settings » Measurements**. |
| **category1-6**         | The **name of the category level** of the **category path of the default category** for the client which is configured in the format settings. |
| **category_concat**     | The **category path of the default category** for the **client** which is configured in the format settings. |
| **image_url_preview**   | The **URL for the image** which is scaled for preview according to the format setting **Image**. |
| **image_url**           | **Required**<br/> The **URL of the image** according to the format setting **Image**. |
| **base_price**          | The **base price information** in the format "price / unit". (e.g.: 10,00 EUR / kilogram) |
| **free_text_field**     | The value of a **property** of type **Text** or **Selection** with a link to **idealo**. |
| **checkoutApproved**    | Is **true** if the order referrer **idealo Direktkauf** within **Items » Edit item » Open item » Open variation » Availability » Markets** is set or a property of type **No** and the link to the idealo Checkout property **CheckoutApproved** is configured. |
| **itemsInStock**        | **Requirement**: checkoutApproved is true.<br/> The **net stock of the variation**. For items which are not limited to the net stock **999** will be exported. |
| **fulfillmentType**     | **Requirement**: checkoutApproved is true.<br/> Property of type **No** with link to one of the options for the idealo Checkout property **FulfillmentType**. |
| **twoManHandlingPrice** | **Requirement**: checkoutApproved is true and fulfillmentType is "Spedition".<br/> Property of type **Text**, **Selection** or **float** and the link to the idealo Checkout property **twoManHandlingPrice**. |
| **disposalPrice**       | **Requirement**: checkoutApproved is true and fulfillmentType is "Spedition".<br/> Property of type **Text**, **Selection** or **float** and the link to the idealo Checkout property **disposalPrice**. |
| **Zahlungsarten**       | **Required**: (min. one payment method)<br/> All payment methods will be exported, according to the format setting **Shipping costs** in its own column. |

_Tab. 2: Columns of the export file_


## 9 Activating the payment method **idealo Checkout**
<a name="Activating the payment method idealo Direktkauf"></a>

Activate the payment method **idealo Checkout**. This allows payments to be made for orders on idealo and to be displayed in your plentymarkets system.

<div class="alert alert-warning" role="alert">
<b>Note: Payment method for idealo Checkout</b><br/> You only have to activate the payment method <b>idealo Checkout</b> if you use idealo Checkout.
 </ul>
</div>

#### Activating the idealo payment method:

1. Go to **Setup » Orders » Payment » Methods**.
2. Place a check mark next to the setting **Also show inactive**.
3. Open the folder **DE > idealo Checkout**.
4. Select the idealo payment method.<br/>
→ The **Settings** tab opens.
5. Carry out the settings as desired. Pay attention to the explanations given in table 2.
6. Place a check mark next to the option **Active**.
7. **Save** the settings.

|**Setting**                        |**Explanation** |
|:---                               |:--- |
|**Language**                       |The following options are saved for the language selected: **Name**, **Info page**, **Info page (internal)**, **Logo**, and **Upload logo**. This enables you to enter values for these options in various languages. The values for a language are activated as soon as a buyer selects the language in the online store. |
|**Name**                           |Enter the name that should be displayed in the online store and on invoices etc. |
|**Info page**                      |Select a category page of the type **content** or enter the URL of a website to provide information about the payment method. |
|**Info page (external)**           |If you selected the option **Info page (external)** under **Info page**, then enter the URL of the info page here. |
|**Countries of delivery**          |Do not select a country of delivery.<br/> You cannot use the payment method in your online store. Therefore, this payment method is only activated in plentymarkets. It is not completely set up. |
|**Logo**                           |Select one of the following options for displaying the logo:<br/> **Show standard logo** = The logo that is saved in plentymarkets for this payment method is displayed.<br/> **Do not show a logo** = The logo that is saved in plentymarkets for this payment method is not displayed.<br/> **Show upload logo** = The options **Logo view** and **Upload logo** are displayed. |
|**Logo view**                      |If **Show upload logo** was selected from the **Logo** drop-down list, then the logo that was uploaded is displayed here. |
|**Upload logo**                    |If **Show upload logo** was selected from the **Logo** drop-down list, then upload an external logo here.<br/> Click on **Upload files** and select the logo that you want to upload for the payment method. Permitted data formats: GIF, PNG, and JPG. |
|**Priority**                       |Select the priority for displaying the payment method in the online store. |
|**Costs: Flat rate or percentage** |If the payment method results in additional costs, enter the percentage value or flat rate value. The choice depends on the conditions of your contract. **Important:** Do not enter a value into both fields.<br/> For further information, refer to the [Managing statistics](https://knowledge.plentymarkets.com/en/basics/working-with-plentymarkets/statistics/managing-statistics) page. For an example of flat rate and percentage costs, refer to the [Managing payment methods](https://knowledge.plentymarkets.com/en/payment/managing-payment-methods#20) page. |

<div class="alert alert-warning" role="alert">
 <b>Permitting the payment method in customer classes</b><br/>
 Go to <b>Setup » CRM » Classes</b> to activate or deactivate permitted payment methods.
 For further information, refer to the [Permitting the payment method in a customer class](https://knowledge.plentymarkets.com/en/payment/managing-payment-methods#30) chapter.
 </ul>
</div>

For further information, refer to the [Managing payment methods](https://knowledge.plentymarkets.com/en/payment/managing-payment-methods) page.

<div class="alert alert-warning" role="alert">
 <b>PayPal payment method</b><br/>
 If you offer the PayPal payment method, it is mandatory to create and configure this payment method in your plentymarkets system. This is to ensure that the payment is imported correctly and assigned to the order.
 </ul>
</div>


## 10 Creating characteristics
<a name="Creating characteristics"></a>
                                       
Use [characteristics](https://knowledge.plentymarkets.com/en/item/settings/properties#100) to link specific characteristics to your items which are required to set up idealo Checkout. Item properties, shipping methods and fees are transferred to idealo Checkout with characteristics.

→ **Note: Characteristics can only be used with the idealo plugin version 2.0**<br/>
The characteristics **DeliveryComment**, **DepositFee**, **DisposalPrice**, **EnergyClass**, **FreeReturnDays**, **Gender**, **Material**, and **Replica** can only be used if the idealo plugin version 2.0 is installed in your plentymarkets system. These characteristics can only be exported to idealo Checkout if you activate the automatic item export. The automatic item export is activated in the **Automatic data transfer** step of the idealo assistant.<br/>
If the automatic item export is activated, you can export all idealo characteristics.<br/>
If you transfer your items with via CSV file with the elastic export, you can only use the characteristic **FulfillmentType**.

### 10.1 Creating the characteristics material and gender

Use the characteristics **Material** and **Gender** to transfer information about material and target group or gender to idealo Checkout.

Proceed as described below to create the characteristic **Material**. Create the **Gender** characteristic in the same way, but select the type **Text** instead.

#### Creating a characteristic for material:

1. Go to **Setup » Item » Characteristics » Tab: New characteristic**.
2. Enter the **Name (internal)**.
3. Select **No** from the characteristic type drop-down list.
4. Select the characteristic **Material** for **idealo Direktkauf property**.
5. **Save** the settings.

Next, you have to link the characteristic to the item in the **Item » Edit item » Open item » Open variation » Tab: Characteristics** menu.

### 10.2 Creating characteristics for shipping methods

With idealo Checkout, the customer buys the items directly at idealo and you have to send shipping information to idealo Checkout. If you ship your items with a parcel service, a shipping company, via letter or via download, this mandatory information is transferred to idealo with a property. If the order is carried out by a shipping company, the customer has to enter their phone number during the order process in order to arrange a delivery date.

Proceed as described below to create the characteristic **FulfillmentType**. This characteristic indicates whether you use the shipping method **shipping company**, **parcel service**, **letter**, or **download**.

#### Creating a characteristic for the shipping method:

1. Go to **Setup » Item » Characteristics » Tab: New characteristic**.
2. Enter the **Name (internal)**.
3. Select **No** from the characteristic type drop-down list.
4. Select the characteristic **FulfillmentType** for **idealo Direktkauf property**.<br/>
→ A drop-down list appears.
5. Select a value from the drop-down list, depending on the shipping type. The values **Spedition** (shipping company), **Paketdienst** (parcel service), **Brief** (letter), and **Download** (download) are available.
6. **Save** the settings.

Next, you have to link the characteristic to the item in the **Item » Edit item » Open item » Open variation » Tab: Characteristics** menu.

#### Further properties for shipping methods

For items which have the shipping method **shipping company**, it is also possible to transfer the additional services **TwoManHandlingPrice** and **DisposalPrice** to idealo Checkout. DisposalPrice can only be used in combination with **TwoManHandlingPrice**. That means you have to create the characteristic **TwoManHandlingPrice** as well as the property **DisposalPrice** and link them to the item. In both cases, select **decimal number** as the characteristic type. Go to **Item » Edit item » Open item » Open variation » Tab: Properties** and enter the surcharge for the additional service with two decimal places behind the decimal separator. Use a period for the decimal separator (19.99).

### 10.3 Creating a characteristic for delivery comments

Use the characteristic **DeliveryComment** to transfer further information about the delivery.

Proceed as described below to create the characteristic **DeliveryComment**.

#### Creating a characteristic to specify further information about the delivery:

1. Go to **Setup » Item » Characteristics » Tab: New characteristic**.
2. Enter the **Name (internal)**.
3. Select **Text** from the characteristic type drop-down list.
4. Select the characteristic **DeliveryComment** for **idealo Direktkauf property**.
5. **Save** the settings.

Next, you have to link the characteristic to the item in the **Item » Edit item » Open item » Open variation » Tab: Characteristics** menu.

### 10.4 Creating the characteristic energy efficiency class

Use the characteristic **EnergyClass** to transfer information about the energy efficiency class to idealo Checkout.

Proceed as described below to create the characteristic **EnergyClass**.

#### Creating a characteristic for the energy efficiency class:

1. Go to **Setup » Item » Characteristics » Tab: New characteristic**.
2. Enter the **Name (internal)**.
3. Select the characteristic type **No** from the characteristic type drop-down list.
4. Select the characteristic **EnergyClass** for **idealo Direktkauf property**.<br/>
→ A drop-down list appears.
5. Select a value from the drop-down list, depending on the energy efficiency class.
6. **Save** the settings.

Next, you have to link the characteristic to the item in the **Item » Edit item » Open item » Open variation » Tab: Characteristics** menu.

### 10.5 Creating the characteristic free return

Use the characteristic **FreeReturnDays** to transfer information about the free return period to idealo Checkout.

Proceed as described below to create the characteristic **FreeReturnDays**.

#### Creating a characteristic for the free return period:

1. Go to **Setup » Item » Characteristics » Tab: New characteristic**.
2. Enter the **Name (internal)**.
3. Select the characteristic type **whole number** from the drop-down list.
4. Select the characteristic **FreeReturnDays** for **idealo Direktkauf property**.
5. **Save** the settings.

Next, you have to link the characteristic to the item in the **Item » Edit item » Open item » Open variation » Tab: Characteristics** menu.

### 10.6 Creating the characteristic deposit fee

Use the characteristic **DepositFee** to transfer information about the deposit fee to idealo Checkout. This characteristic is required if a deposit fee must be paid for an item.

Proceed as described below to create the characteristic **DepositFee**.

#### Creating the characteristic deposit fee:

1. Go to **Setup » Item » Characteristics » Tab: New characteristic**.
2. Enter the **Name (internal)**.
3. Select the characteristic type **decimal number** from the drop-down list.
4. Select the characteristic **DepositFee** for **idealo Direktkauf property**.
5. **Save** the settings.

Next, you have to link the characteristic to the item in the **Item » Edit item » Open item » Open variation » Tab: Characteristics** menu.

### 10.7 Creating the characteristic replica

Use the characteristic **Replica** to specify whether the item is a replica.

Proceed as described below to create the characteristic **Replica**.

#### Creating the characteristic replica:

1. Go to **Setup » Item » Characteristics » Tab: New characteristic**.
2. Enter the **Name (internal)**.
3. Select the characteristic type **No** from the characteristic type drop-down list.
4. Select the characteristic **Replica** for **idealo Direktkauf property**.
5. **Save** the settings.

Next, you have to link the characteristic to the item in the **Item » Edit item » Open item » Open variation » Tab: Characteristics** menu.

## 11 Setting up event procedures
<a name="Setting up event procedures"></a>

Set up event procedures to automatically inform idealo about changes in the order status. You can use event procedures to automatically send order confirmations, shipping confirmations, returns, and cancellations to idealo Checkout.

<div class="alert alert-warning" role="alert">
 <b>Note: Event procedures for idealo Checkout</b><br/>
 You only have to set up event procedures if you use idealo Checkout.
 </ul>
</div>

### 11.1 Automatically sending order confirmations

Set up an [event procedure](https://knowledge.plentymarkets.com/en/automation/event-procedures) to automatically send an order confirmation to idealo.

#### Setting up an event procedure:

1. Go to **Setup » Orders » Events**.
2. Click on **Add event procedure**.<br/>
→ The **Create new event procedure** window opens.
3. Enter a name.
4. Select the event listed in Table 3 below.
5. **Save** the settings.<br/>
→ The event is created.
6. Carry out further settings. Pay attention to the explanations given in Table 3 below.
7. Place a check mark next to the option **Active**.
8. **Save** the settings.<br/>
→ The event procedure is saved.

|**Setting** |**Option**                                    |**Selection** |
|:---        |:---                                          |:--- |
|Event       |**Order generation: New order**               | |
|Filter 1    |**Order > Order type**                        |**Order** |
|Filter 2    |**Order > Referrer**                          |**idealo Checkout** |
|Procedure   |**Order > Send order confirmation to idealo** | |

### 11.2 Automatically sending shipping confirmations

Set up an [event procedure](https://knowledge.plentymarkets.com/en/automation/event-procedures) to automatically send a shipping confirmation to idealo when the outgoing items have been booked.

#### Setting up an event procedure:

1. Go to **Setup » Orders » Events**.
2. Click on **Add event procedure**.<br/>
→ The **Create new event procedure** window opens.
3. Enter a name.
4. Select the event listed in Table 4 below.
5. **Save** the settings.<br/>
→ The event is created.
6. Carry out further settings. Pay attention to the explanations given in Table 4.
7. Place a check mark next to the option **Active**.
8. **Save** the settings.<br/>
→ The event procedure is saved.

|**Setting** |**Option**                                          |**Selection** |
|:---        |:---                                                |:--- |
|Event       |**Order change: Outgoing items booked**             | |
|Filter 1    |**Order > Order type**                              |**Order** |
|Filter 2    |**Order > Referrer**                                |**idealo Checkout** |
|Procedure   |**Shipping > Send shipping confirmation to idealo** | |

### 11.3 Automatically sending returns

Set up an [event procedure](https://knowledge.plentymarkets.com/en/automation/event-procedures) to automatically inform idealo about returns.

#### Setting up an event procedure:

1. Go to **Setup » Orders » Events**.
2. Click on **Add event procedure**.<br/>
→ The **Create new event procedure** window opens.
3. Enter a name.
4. Select the **event** listed in Table 5.
5. **Save** the settings.<br/>
→ The event is created.
6. Carry out further settings. Pay attention to the explanations given in Table 5.
7. Place a check mark next to the option **Active**.
8. **Save** the settings.<br/>
→ The event procedure is saved.

|**Setting** |**Option**                         |**Selection** |
|:---        |:---                               |:--- |
|Event       |**Order generation: New return**   | |
|Filter 1    |**Order > Order type**             |**Return** |
|Filter 2    |**Order > Referrer**               |**idealo Checkout** |
|Procedure   |**Return > Send return to idealo** | |

### 11.4 Automatically sending cancellations

Set up an [event procedure](https://knowledge.plentymarkets.com/en/automation/event-procedures) to automatically inform idealo of cancellations.

#### Setting up an event procedure:

1. Go to **Setup » Orders » Events**.
2. Click on **Add event procedure**.<br/>
→ The **Create new event procedure** window opens.
3. Enter a name.
4. Select the event listed in Table 6.
5. **Save** the settings.<br/>
→ The event is created.
6. Carry out further settings. Pay attention to the explanations given in Table 6.
7. Select a reason for the cancellation.
8. Place a check mark next to the option **Active**.
9. **Save** the settings.<br/>
→ The event procedure is saved.

|**Setting** |**Option**                             |**Selection** |
|:---        |:---                                   |:--- |
|Event       |**Status change: [8] Cancelled**       | |
|Filter 1    |**Order > Order type**                 |**Order** |
|Filter 2    |**Order > Referrer**                   |**idealo Checkout** |
|Procedure   |**Order: Send cancellation to idealo** | |


## 12 Viewing the API log

The **Data » API log** menu contains a history of processes that run via the idealo interface. The **idealoDirektkauf** format is available for idealo.

#### Viewing the API log:

1. Go to **Data » API-Log » Tab: API log**.
2. Select the format **idealoDirektkauf** from the **Process** drop-down list.
3. Select a **date** if you only want to see entries for a specific day.
4. Select the number of results per page.
5. Click on **Search** to display the results.


## 13 Licence

This project is licensed under the GNU AFFERO GENERAL PUBLIC LICENSE.- find further information in the [LICENSE.md](https://github.com/plentymarkets/plugin-elastic-export-idealo-de/blob/master/LICENSE.md).